<template>
  <div class="music-playlist">
    <div class="header">
      <h2 class="header__title">playlist</h2>
      <SearchItem />
    </div>
    <ArtistsListItem  
      v-for="item in artists" :key="item.id" :artist="item"
    />
  </div>
</template>

<script>
import SearchItem from './items/SearchItem.vue';
import ArtistsListItem from './items/ArtistsListItem.vue';

export default {
  name: 'MusicPlaylistSection',
  components: {
    SearchItem,
    ArtistsListItem,
  },
  data() {
    return {
      artists: [
        {
          id:1,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
        {
          id:2,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
        {
          id:3,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
        {
          id:4,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
        {
          id:5,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
        {
          id:6,
          img: 'received_909123655824827.jpeg',
          songName: 'Polska',
          artist: 'Kazik',
          durationOfSong: '5:24',
          rate: 0,
        },
      ]
    }
  },
}
</script>

<style lang="scss" scoped>
.music-playlist{
  margin: 140px 0 100px 0;
}
.header{
  position: fixed;
  top: 0;
  left:0;
  right:0;
  padding: 20px 0;
  text-align: center;
  background-color: #202740;
  margin-bottom: 15px;

  &__title{
    font-size: 25px;
    color: #3DC864;
    font-family:'Arial Narrow', Arial, sans-serif;
    text-transform: uppercase;    
    letter-spacing: 2px;
    font-weight: lighter;
    margin-bottom: 15px;
  }
}
</style>