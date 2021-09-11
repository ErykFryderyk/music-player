<template>
  <div class="">
    <Navigator 
      @show-users="visibleUsers = !visibleUsers"
      @show-playlist="visiblePlaylist = !visiblePlaylist"
      />
    <UsersList v-show="visibleUsers"/>
    <Playlist @change="visibleUsers = !visibleUsers"
      v-show="visiblePlaylist"/>
  </div>
</template>

<script>
import Navigator from './components/Navigator.vue';
import UsersList from './components/Users.vue';
import Playlist from './components/Playlist.vue';

export default {
  name: 'App',
  components: {
    Navigator,
    UsersList,
    Playlist,
  },
  data() {
    return {
        visibleUsers: false,
        visiblePlaylist: false,
    }
  },
  methods: {
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
