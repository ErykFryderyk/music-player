<template>
  <div class="container">
      <div class="header">
          <h1 class="header__title">Party Peaple</h1>
      </div>
      <div class="users">
        <ul class="users__list">
            <li class="users__item">
                <img class="users__avatar" src="../assets/received_909123655824827.jpeg" alt="">
                <p class="users__name">AnitaBus</p>
            </li>
            <li class="users__item">
                <img class="users__avatar" src="../assets/received_909123655824827.jpeg" alt="">
                <p class="users__name">AnitaBus</p>
            </li>
            <li class="users__item">
                <img class="users__avatar" src="../assets/received_909123655824827.jpeg" alt="">
                <p class="users__name">AnitaBus</p>
            </li>
            <li class="users__item">
                <img class="users__avatar" src="../assets/received_909123655824827.jpeg" alt="">
                <p class="users__name">AnitaBus</p>
            </li>
            <li class="users__item">
                <img class="users__avatar" src="../assets/received_909123655824827.jpeg" alt="">
                <p class="users__name">AnitaBus</p>
            </li>
            <li class="users__item">
                <img class="users__avatar" src="../assets/received_909123655824827.jpeg" alt="">
                <p class="users__name">AnitaBus</p>
            </li>
        </ul>
      </div>
  </div>
</template>

<script>
export default {
    name: 'users-list',
}
</script>

<style lang="scss" scoped>
.container{
    background-color: #282F46;
    width: 100%;
    height: 100vh;
    position: relative;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: 1;
}
.header{
    text-align: center;
    padding: 20px 0px;
    width: 100%;
    top: 0;
    position: fixed;
    background-color: #282F46;
    border-bottom: 1px solid #3dc86473;

    &__title{
        font-size: 25px;
        color: #3DC864;
        font-family:'Arial Narrow', Arial, sans-serif;
        text-transform: uppercase;    
        letter-spacing: 2px;
        font-weight: lighter;
    }
}
.users{
    margin:75px 0;

    &__item{
        display:flex;
        align-items: center;
        padding: 10px;
        padding-left:20px;

        &:nth-child(odd){
            background-color: rgba(0, 0, 0, 0.08);
        }
    }
    &__list{

    }

    &__avatar{
        width: 70px;
        height: 70px;
        border-radius: 50%;
    }
    &__name{
        margin-left: 15px;
        font-size: 22px;
        font-family: 'Franklin Gothic', 'Arial Narrow', Arial, sans-serif;
        letter-spacing: 1px;
    }
}
</style>