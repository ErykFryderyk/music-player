<template>
    <div class="search-box">
        <input type="text" class="search-box__input" placeholder="Search">
        <button class="search-box__btn">
          <svg width="28" height="34" viewBox="0 0 28 34" fill="transparent" xmlns="http://www.w3.org/2000/svg">
          <circle cx="12" cy="12" r="11" stroke="#3DC864" stroke-width="2"/>
          <line x1="18.8517" y1="20.4759" x2="26.8517" y2="33.4759" stroke="#3DC864" stroke-width="2"/>
          </svg>
      </button>
    </div>
</template>

<script>

export default {
  name: 'SearchItem',
}
</script>

<style lang="scss" scoped>
.search-box {
    margin: 0 15px;
    display: flex;
    justify-content: center;
    align-items: center;

    &__input{
        height: 45px;
        width: 100%;
        font-size: 20px;
        letter-spacing: 1px;
        padding-left: 10px;
        color: #fff;
        background-color: transparent;
        border:none;
        border-bottom: 2px solid #3DC864;
        border-top: 2px solid #3DC864;
        font-family: 'Arial Narrow', Arial, sans-serif;
        outline: none;

        &::placeholder{
            font-size: inherit;
            color: #fff;
        }
    }
    &__btn{
        border: none;
        border-bottom: solid 2px #3DC864;
        border-top: solid 2px #3DC864;
        height: 45px;
        width: 50px;
        cursor: pointer;
        background-color: transparent;
        outline: none;
        -webkit-tap-highlight-color: transparent;

        svg{
            width: 100%;
            height: 30px;
        }
    }
}
</style>