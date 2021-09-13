<template>
  <div class="playlist">
      <div class="header">
          <h2 class="header__title">playlist</h2>
          <div class="search-box">
              <input type="text" class="search-box__input" placeholder="Search">
              <button class="search-box__btn">
                <svg width="28" height="34" viewBox="0 0 28 34" fill="transparent" xmlns="http://www.w3.org/2000/svg">
                <circle cx="12" cy="12" r="11" stroke="#3DC864" stroke-width="2"/>
                <line x1="18.8517" y1="20.4759" x2="26.8517" y2="33.4759" stroke="#3DC864" stroke-width="2"/>
                </svg>
            </button>
          </div>
      </div>
      <div class="playlist-box">
          <ul class="playlist-box__list">
              <li class="playlist-item">
                    <img class="playlist-item__image" src="../assets/received_909123655824827.jpeg" alt="">
                    <div class="playlist-item__song">
                        <h3 class="playlist-item__song-name">Polska</h3>
                        <h4 class="playlist-item__artist">Kazik</h4>
                    </div>
                    <div class="playlist-item__info">
                        <span class="playlist-item__time">5:24</span>
                        <span class="plalist-item__rate">******</span>
                    </div>
              </li>
              <li class="playlist-item">
                    <img class="playlist-item__image" src="../assets/received_909123655824827.jpeg" alt="">
                    <div class="playlist-item__song">
                        <h3 class="playlist-item__song-name">Polska</h3>
                        <h4 class="playlist-item__artist">Kazik</h4>
                    </div>
                    <div class="playlist-item__info">
                        <span class="playlist-item__time">5:24</span>
                        <span class="plalist-item__rate">******</span>
                    </div>
              </li>
              <li class="playlist-item">
                    <img class="playlist-item__image" src="../assets/received_909123655824827.jpeg" alt="">
                    <div class="playlist-item__song">
                        <h3 class="playlist-item__song-name">Polska</h3>
                        <h4 class="playlist-item__artist">Kazik</h4>
                    </div>
                    <div class="playlist-item__info">
                        <span class="playlist-item__time">5:24</span>
                        <span class="plalist-item__rate">******</span>
                    </div>
              </li>
              <li class="playlist-item">
                    <img class="playlist-item__image" src="../assets/received_909123655824827.jpeg" alt="">
                    <div class="playlist-item__song">
                        <h3 class="playlist-item__song-name">Polska</h3>
                        <h4 class="playlist-item__artist">Kazik</h4>
                    </div>
                    <div class="playlist-item__info">
                        <span class="playlist-item__time">5:24</span>
                        <span class="plalist-item__rate">******</span>
                    </div>
              </li>
              <li class="playlist-item">
                    <img class="playlist-item__image" src="../assets/received_909123655824827.jpeg" alt="">
                    <div class="playlist-item__song">
                        <h3 class="playlist-item__song-name">Polska</h3>
                        <h4 class="playlist-item__artist">Kazik</h4>
                    </div>
                    <div class="playlist-item__info">
                        <span class="playlist-item__time">5:24</span>
                        <span class="plalist-item__rate">******</span>
                    </div>
              </li>
              <li class="playlist-item">
                    <img class="playlist-item__image" src="../assets/received_909123655824827.jpeg" alt="">
                    <div class="playlist-item__song">
                        <h3 class="playlist-item__song-name">Polska</h3>
                        <h4 class="playlist-item__artist">Kazik</h4>
                    </div>
                    <div class="playlist-item__info">
                        <span class="playlist-item__time">5:24</span>
                        <span class="plalist-item__rate">******</span>
                    </div>
              </li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    name: 'playlist',
    data() {
        return {

        }
    },
    methods: {

    },
}
</script>

<style lang="scss" scoped>
.playlist{
    background-color: #282F46;
    position: relative;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: 1;
}
.header{
padding: 20px 0;
text-align: center;
background-color: #202740;
margin-bottom: 15px;

    &__title{
        font-size: 25px;
        color: #3DC864;
        font-family:'Arial Narrow', Arial, sans-serif;    
        text-transform: uppercase;    
        letter-spacing: 2px;
        font-weight: lighter;
        margin-bottom: 15px;
    }
}
.search-box {
    margin: 0 15px;
    display: flex;
    justify-content: center;
    align-items: center;

    &__input{
        height: 45px;
        width: 100%;
        font-size: 20px;
        letter-spacing: 1px;
        padding-left: 10px;
        color: #fff;
        background-color: transparent;
        border:none;
        border-bottom: 2px solid #3DC864;
        border-top: 2px solid #3DC864;
        font-family: 'Arial Narrow', Arial, sans-serif;
        outline: none;

        &::placeholder{
            font-size: inherit;

            color: #fff;
        }
    }
    &__btn{
        border: none;
        border-bottom: solid 2px #3DC864;
        border-top: solid 2px #3DC864;
        height: 45px;
        width: 50px;
        cursor: pointer;
        background-color: transparent;
        outline: none;
        -webkit-tap-highlight-color: transparent;

        svg{
            width: 100%;
            height: 30px;
        }
    }
}
.playlist-box{
    margin: 0 20px;
}
.playlist-item{
    display: flex;
    align-items: center;

    &__image{
        height: 75px;
        border-radius: 20px;
    }

    &__song{
        margin-left: 10px;
        width: 100%;
        height: 100px;
        display: flex;
        justify-content: center;
        flex-direction: column;
        line-height: 1.5;
    }

    &__song-name{
        font-family: 'Franklin Gothic', 'Arial Narrow', Arial, sans-serif;
        font-size: 22px;
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

</style>