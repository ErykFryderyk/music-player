<template>
  <div class="users-list">
    <div class="header">
      <h2 class="header__title">party peaple</h2>
    </div>
    <UsersList 
      v-for="user in users" :key="user.id" :user="user"
    />
  </div>
</template>

<script>
import UsersList from './items/UsersList.vue';
export default {
  name: 'PartyPeaple',
  components: {
    UsersList,
  },
  data() {
    return {
      users: [
      {
        id: Math.random(),
        userName: 'Antonina Kobylarek',
        avatarImage: '',
      },
      {
        id: Math.random(),
        userName: 'Antonina Kobylarek',
        avatarImage: '',
      },
      {
        id: Math.random(),
        userName: 'Antonina Kobylarek',
        avatarImage: '',
      },
      {
        id: Math.random(),
        userName: 'Antonina Kobylarek',
        avatarImage: '',
      },
     ]
    }
  },
}
</script>

<style lang="scss" scoped>
.users-list{
  margin: 70px 0 100px 0;
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
</style>