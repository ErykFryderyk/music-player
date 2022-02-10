<template>
  <div class="favorite-song">
    <div class="favorite-song__item">
      <img class="song-box__image" src="../../assets/received_909123655824827.jpeg" alt="">
      <div class="song-box__song">
        <h3 class="__song-name">Polska</h3>
        <h4 class="__artist">Kazik</h4>
      </div>
    </div>
    <div class="favorite-song__item favorite-song__item--flex-column">
      <span class="song-time">5:24</span>
      <div class="rating">
        <span class="rating__circle rating__circle--checked"></span>
        <span class="rating__circle rating__circle--checked"></span>
        <span class="rating__circle rating__circle--checked"></span>
        <span class="rating__circle"></span>
        <span class="rating__circle"></span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FavoriteSong',
  data(){
    return{

    }
  }
}
</script>

<style lang="scss" scoped>
.favorite-song{
  width: 100%;
  background-color: #1d23364d;
  display:flex;
  margin-bottom: 20px;
  padding: 16px 20px;
  justify-content: space-between;
  align-items: center;

  &__item{
    display: flex;
    align-items: center;

    &--flex-column{
      flex-direction: column;
    }
  }
}
.song-time{
    margin-bottom: 5px;
    font-size: 20px;
}
.song-box{
  &__inner{
      display: flex;
      align-items: center;
  }

  &__image{
      height:80px;
      width: 80px;
      border-radius: 20px ;
  }
  &__song{
      margin-left:10px;
  }
  &__info{
      display: flex;
      flex-direction: column;
      text-align: right;
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