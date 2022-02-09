<template>
  <div class="music-playlist">
    <div class="header">
      <h2 class="header__title">playlist</h2>
      <SearchItem />
    </div>
    <ArtistsListItem />
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
  }
}
</script>

<style lang="scss" scoped>
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