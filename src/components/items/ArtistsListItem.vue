<template>
  <div class="playlist-box">
    <ul>
      <li class="playlist-item">
        <div class="playlist-item__box">
          <img class="playlist-item__image" src="../../assets/received_909123655824827.jpeg" alt="">
          <div class="playlist-item__song">
            <h3 class="playlist-item__song-name">{{artist.songName}}</h3>
            <h4 class="playlist-item__artist">{{artist.artist}}</h4>
          </div>
        </div>
        <div class="playlist-item__info">
          <span class="playlist-item__time">{{artist.durationOfSong}}</span>
          <div class="rating">
            <span class="rating__circle rating__circle--checked"></span>
            <span class="rating__circle rating__circle--checked"></span>
            <span class="rating__circle rating__circle--checked"></span>
            <span class="rating__circle"></span>
            <span class="rating__circle"></span>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'ArtistsListItem',
  props: {
    artist: Object,

  },
  data() {
    return{
    }
  }
}
</script>

<style lang="scss" scoped>
.playlist-box{
  margin: 0px 20px;
}
.playlist-item{
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 20px;

  &__box{
    display: flex;
    align-items: center;
  }

  &__image{
    width: 75px;
    border-radius: 20px;
  }
  &__song{
    margin-left: 10px;
  }
  &__artist{
    font-family: 'Franklin Gothic', 'Arial Narrow', Arial, sans-serif;
    font-size: 18px;
  }
  &__info{
    display: flex;
    justify-content: center;
    flex-direction: column;
    line-height: 1.5;
    text-align: right;
  }

  &__time{
    font-size: 20px;
    font-family: 'Franklin Gothic';
  }
  &__rate{
    font-size: 20px;
    font-family: 'Franklin Gothic';
  }
}
.rating{
  width: 70px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  &__circle{
    height: 9px;
    width: 9px;
    background-color: #969696;
    border-radius: 50%;
    cursor:pointer;

    &--checked{
      width: 10px;
      height: 10px;
      background-color: #fff;
    }
  }

}
</style>