<template>
  <div class="next-song">
    <div class="next-song__header">
      <h3 class="next-song__title">Next song</h3>
    </div>
    <div>
      <ul class="next-song__list">
        <li class="next-song__list-item">
          <div class="">
            <h2>{{nextSong.songName}}</h2>
            <h4>{{nextSong.artist}}</h4>
          </div>
          <p class="result-of-the-vote"><span class="like">{{nextSong.likes}}</span> | <span class="dislike">{{nextSong.disLikes}}</span></p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'WonSong',
  props: {
    nextSong: Object,
  },
  data(){
    return{
    }
  }
}
</script>

<style lang="scss" scoped>
.next-song{
    width: 100%;
    margin-bottom: 20px;

    &__header{
      margin-bottom: 10px;
    }

    &__list-item{
      background: #00000040;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 9px;
      margin-bottom: 10px;
    }
}
.result-of-the-vote{
  font-size: 16px;

  .like{
    color: #3ea73e;
  }
  .dislike{
    color: #df2f2f;
  }
}
</style>