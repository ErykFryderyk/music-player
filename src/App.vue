<template>
  <div class="container">
    <Navigator 
      @show-users="visibleUsers = !visibleUsers"
      @show-playlist="visiblePlaylist = !visiblePlaylist"
      />
    <UsersList v-show="visibleUsers"/>
    <Playlist @change="visibleUsers = !visibleUsers"
      v-show="visiblePlaylist"/>
    <Player v-show="visiblePlayer"/>
  </div>
</template>

<script>
import Navigator from './components/Navigator.vue';
import UsersList from './components/Users.vue';
import Playlist from './components/Playlist.vue';
import Player from './components/Player.vue';

export default {
  name: 'App',
  components: {
    Navigator,
    UsersList,
    Playlist,
    Player,
  },
  data() {
    return {
        visibleUsers: false,
        visiblePlaylist: false,
        visiblePlayer: false,
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
  font-family: 'Franklin Gothic', 'Arial Narrow', Arial, sans-serif;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  margin: 0;
  padding: 0;
  font-weight: normal;
  line-height: normal;
  font-size: 18px;
  color: white; }

ul {
  padding: 0;
  margin: 0; }

li {
  margin: 0;
  padding: 0;
  list-style: none;
  color: white; }

a {
  text-decoration: none;
  color: white; }

p {
  font-size: 16px;
  color: white;
  line-height: 1.5;
  letter-spacing: 1px; }

img {
  max-width: 100%; 
}
.container{
  width: 100%;

}
</style>
