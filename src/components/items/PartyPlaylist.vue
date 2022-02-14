<template>
  <div class="party-playlist">
    <div class="party-playlist__header">
      <h3 class="party-playlist__title">Party playlist</h3>
    </div>
    <div class="party-playlist__list">
      <ul class="list-of-songs"
        v-for="i in item" :key="i.id">
        <li class="list-of-songs__item">
          <div class="">
            <p>{{i.song}}</p>
            <p>{{i.artist}}</p>
          </div>
          <div class="rate-buttons">
            <button class="rate-btn rate-btn--like">Like</button>
            <button class="rate-btn rate-btn--hate">Unlike</button>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PartyPlaylist',
  props: {
    item: Object,
  },
  data() {
    return{
    }
  }
}
</script>

<style lang="scss" scoped>
.party-playlist{
  background-color: transparent;
  
  &__header{
    margin-bottom: 15px;
  }
  &__title{
    font-size: 22px;
  }
}

.list-of-songs{
  width: 100%;

  &__item{
    background: #00000040;
    display: flex;
    justify-content: space-between;
    padding: 9px;
    margin-bottom: 10px;
  }
}

.rate-buttons{
  width: 50px;
  display: flex;
  justify-content: space-between;
}

.rate-btn{
  background: transparent;
  border:none;
  cursor: pointer;
  text-align: center;

  &--like{
      border: 2px solid green;
      color: green;
  }
  &--hate{
      border: 2px solid red;
      color: red;
  }
    }
</style>