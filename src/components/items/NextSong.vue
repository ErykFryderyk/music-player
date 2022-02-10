<template>
  <div class="next-song">
    <div class="next-song__header">
      <h3 class="next-song__title">Next song</h3>
    </div>
    <div>
      <ul class="next-song__list">
        <li class="next-song__list-item">
          <span>{{nextSong.artist}} - {{nextSong.song}}</span>
          <p class="result-of-the-vote"><span class="like">23</span> / <span class="unlike">2</span></p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'WonSong',
  data(){
    return{
      nextSong: {
        artist: 'Queen Of The Stone Age',
        song: 'In The Fade',
      }
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
    color: green;
  }
  .unlike{
    color: red;
  }
}
</style>