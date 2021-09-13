<template>
  <div class="wrapper">
      <div class="song-box">
            <img class="song-box__image" src="../assets/received_909123655824827.jpeg" alt="">
            <div class="song-box__song">
                <h3 class="__song-name">Polska</h3>
                <h4 class="__artist">Kazik</h4>
            </div>
            <div class="song-box__info">
                <span class="__time">5:24</span>
                <span class="__rate">******</span>
            </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'player',
    data() {
        return {

        }
    }


}
</script>

<style lang="scss" scoped>
    .wrapper{
        width: 100%;
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background-color: #fff;
    }
    .song-box{
        width: 300px;
        // height: 300px;
        padding: 20px;
        border: 1px solid white;
        display:flex;
        justify-content: center;
        align-items: center;

        &__image{
            height: 100px;
            width: 100px;
            border-radius: 30px ;
        }
        &__song{
            margin-left:10px;

        }
    }

</style>