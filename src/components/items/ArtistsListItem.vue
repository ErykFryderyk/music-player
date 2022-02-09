<template>
  <div class="playlist-box">
    <ul>
      <li v-for="item in artists" :key="artists.id" class="playlist-item">
        <div class="playlist-item__box">
          <img class="playlist-item__image" src="../../assets/received_909123655824827.jpeg" alt="">
          <div class="playlist-item__song">
            <h3 class="playlist-item__song-name">{{item.songName}}</h3>
            <h4 class="playlist-item__artist">{{item.artist}}</h4>
          </div>
        </div>
        <div class="playlist-item__info">
          <span class="playlist-item__time">{{item.durationOfSong}}</span>
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
  data() {
    return{
      artists: [
        {
          id:1,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
        {
          id:2,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
        {
          id:3,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
        {
          id:4,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
        {
          id:5,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
        {
          id:6,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.playlist-box{
  margin: 150px 20px 100px 20px;
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