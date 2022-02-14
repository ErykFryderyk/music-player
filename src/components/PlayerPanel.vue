<template>
  <div class="player-panel">
    <FavoriteSongToPlay />
    <NextSong />
    <PartyPlaylist 
      :item="songs"
    />
  </div>
</template>

<script>
import FavoriteSongToPlay from './items/FavoriteSongToPlay.vue';
import NextSong from './items/NextSong.vue';
import PartyPlaylist from './items/PartyPlaylist.vue';

export default {
  name: 'PlayerPanel',
  components: {
    FavoriteSongToPlay,
    NextSong,
    PartyPlaylist,
  },
  data() {
    return {
      songs: [
        {
          id: Math.random(),
          artist: 'Queen Of The Stone Age',
          song: 'In The Fade',
        },
        {
          id: Math.random(),
          artist: 'Queen Of The Stone Age',
          song: 'In The Fade',
        },
        {
          id: Math.random(),
          artist: 'Queen Of The Stone Age',
          song: 'In The Fade',
        },
        {
          id: Math.random(),
          artist: 'Queen Of The Stone Age',
          song: 'In The Fade',
        },
      ],
    }
  },
}
</script>

<style lang='scss' scoped>
  .player-panel{
    width: 100%;
    min-height: 100vh;
    padding-left: 15px;
    padding-right: 15px;
    margin-left: auto;
    margin-right: auto;
    background: rgb(50,89,36);
    background: linear-gradient(180deg, rgba(50,89,36,1) 0%, rgba(16,21,35,1) 76%);
  }
</style>