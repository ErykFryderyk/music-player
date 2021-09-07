<template>
  <div class="">
    <Navigator/>
    <UsersList/>
  </div>
</template>

<script>
import Navigator from './components/Navigator.vue';
import UsersList from './components/Users.vue';

export default {
  name: 'App',
  components: {
    Navigator,
    UsersList,
  },
  data() {
    return {
    }
  }
}
</script>

<style lang="scss">
*, *::before, *::after{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
body{
  background-color: #282F46;
  color: #fff;
}
</style>
