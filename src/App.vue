<template>
  <div class="container">
    <Navigator 
      @show-users="showModal"
      @show-playlist="showModal"
      @show-player="showModal"
      />
    <UsersList v-show="visibleModals.visibleUsers"/>
    <Playlist v-show="visibleModals.visiblePlaylist"/>
    <Player v-show="visibleModals.visiblePlayer"/>
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
      visibleModals: {
        visibleUsers: false,
        visiblePlaylist: false,
        visiblePlayer: true,
      }
    }
  },
  methods: {
    showModal(el) {
      for(let prop in this.visibleModals) {
        this.visibleModals[prop] = false;
        if(el === prop){
          this.visibleModals[prop] = true;
        }
      }
    }
  }
}
</script>

<style lang="scss">
*, *::before, *::after{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  -webkit-tap-highlight-color: transparent;
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
