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
            <LikeBtn :isLike="true">
              <font-awesome-icon icon="heart" />
            </LikeBtn>
            <LikeBtn :isLike="false">
              <font-awesome-icon icon="thumbs-down" />
            </LikeBtn>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import LikeBtn from '../items/LikeBtn.vue';

export default {
  name: 'PartyPlaylist',
  components: {
    LikeBtn,
  },
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
  width: 70px;
  display: flex;
  justify-content: space-between;
  align-items: center;
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