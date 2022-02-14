<template>
  <div class="users">
    <ul class="users__list">
      <li class="users__item">
        <img class="users__avatar" src="../../assets/received_909123655824827.jpeg" alt="">
        <p class="users__name">{{user.userName}}</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
 name: 'UsersList',
 props: {
   user: Object,
 },
 data() {
   return{
   }
 }
}
</script>

<style lang='scss' scoped>
.users{

    &__item{
        display:flex;
        align-items: center;
        padding: 10px;
        padding-left:10px;

    }
    &__list{
      .users__list:nth-child(odd){
        background-color: rgba(0, 0, 0, 0.08);
      }
    }

    &__avatar{
        width: 70px;
        height: 70px;
        border-radius: 50%;
    }
    &__name{
        margin-left: 20px;
        font-size: 22px;
        font-family: 'Franklin Gothic', 'Arial Narrow', Arial, sans-serif;
        letter-spacing: 1px;
    }
}
</style>