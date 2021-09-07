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

<style lang="scss">
.container{
    background-color: #282F46;
    width: 100%;
    height: 100vh;
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
        font-size: 35px;
        color: #3DC864;
    }
}
.users{
    margin-top: 100px;

    &__item{
        display:flex;
        align-items: center;
        margin-bottom: 15px;
    }
    &__list{
        margin-left: 30px;
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