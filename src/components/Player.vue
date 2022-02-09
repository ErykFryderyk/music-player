<template>
    <div class="header">
        <h1 class="header__title">Player</h1>
    </div>
    <div class="wrapper">
        <div class="song-box">
            <div class="song-box__inner">
                <img class="song-box__image" src="../assets/received_909123655824827.jpeg" alt="">
                <div class="song-box__song">
                    <h3 class="__song-name">Polska</h3>
                    <h4 class="__artist">Kazik</h4>
                </div>
            </div>
            <div class="song-box__info">
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
        <div class="next-song">
            <div class="">
                <h3 class="next-song__title">Next song</h3>
                <ul class="next-song__list">
                    <li class="next-song__list-item">
                        <span>{{songs[0].artist}} - {{songs[0].song}}</span>
                        <div class="rate-buttons">
                            <button class="rate-btn rate-btn--like">4</button>
                            <button class="rate-btn rate-btn--hate">2</button>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
        <div class="party-playlist">
            <h3 class="party-playlist__title">Party playlist</h3>
            <ul class="next-song__list">
                <li class="next-song__list-item">
                    <span>{{songs[0].artist}} - {{songs[0].song}}</span>
                    <div class="rate-buttons">
                        <button class="rate-btn rate-btn--like">4</button>
                        <button class="rate-btn rate-btn--hate">2</button>
                    </div>
                </li>
                <li class="next-song__list-item">
                    <span>{{songs[0].artist}} - {{songs[0].song}}</span>
                    <div class="rate-buttons">
                        <button class="rate-btn rate-btn--like">4</button>
                        <button class="rate-btn rate-btn--hate">2</button>
                    </div>
                </li>
                <li class="next-song__list-item">
                    <span>{{songs[0].artist}} - {{songs[0].song}}</span>
                    <div class="rate-buttons">
                        <button class="rate-btn rate-btn--like">4</button>
                        <button class="rate-btn rate-btn--hate">2</button>
                    </div>
                </li>
                <li class="next-song__list-item">
                    <span>{{songs[0].artist}} - {{songs[0].song}}</span>
                    <div class="rate-buttons">
                        <button class="rate-btn rate-btn--like">4</button>
                        <button class="rate-btn rate-btn--hate">2</button>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'player',
    props: [

    ],
    data() {
        return {
            songs: [
                {
                    artist: 'Kazik',
                    song: 'Polska',
                },
                {
                    artist: 'Kazik',
                    song: 'Polska',
                },
                {
                    artist: 'Kazik',
                    song: 'Polska',
                },
                {
                    artist: 'Kazik',
                    song: 'Polska',
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
    .wrapper{
        width: 100%;
        min-height: 100vh;
        display: flex;
        align-items: center;
        flex-direction: column;
        position: absolute;
        padding: 15px;
        background: rgb(50,89,36);
        background: linear-gradient(180deg, rgba(50,89,36,1) 0%, rgba(16,21,35,1) 76%);
    }
    .song-box{
        width: 100%;
        background-color: #1d23364d;
        display:flex;
        padding: 16px 20px;
        justify-content: space-between;
        align-items: center;
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
    .next-song, 
    .party-playlist{
        width: 100%;
        padding: 15px 0;

        &__title{
            font-size: 22px;
            margin:  0 0 15px 10px;
        }
        &__list{
        }
        &__list-item{
            background: #00000040;
            display: flex;
            justify-content: space-between;
            padding: 9px;
            padding-left: 20px;
            margin-bottom: 10px;
        }
    }
    .song-time{
        margin-bottom: 5px;
        font-size: 20px;

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
    .rate-buttons{
        width: 50px;
        display: flex;
        justify-content: space-between;
    }
    .rate-btn{
        width: 20px;
        height: 20px;
        background: transparent;
        border:none;
        border-radius:50%;
        cursor: pointer;
        text-align: center;

        &--like{
            border: 2px solid green;
            color: green;
        }
        &--hate{
            border: 2px solid red;
            color: red;
        }
    }
</style>