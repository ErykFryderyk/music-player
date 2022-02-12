<template>
  <div class="users-list">
    <div class="header">
      <h2 class="header__title">party peaple</h2>
    </div>
    <UsersList/>
  </div>
</template>

<script>
import UsersList from './items/UsersList.vue';
export default {
  name: 'PartyPeaple',
  components: {
    UsersList,
  }
}
</script>

<style lang="scss" scoped>
.party-peaple{}
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