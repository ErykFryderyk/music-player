<template>
  <div class="navigation">
      <button @click="$emit('show-users')">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M7 5h14v2H7z"/><circle cx="4" cy="6" r="1.5"/><path d="M7 11h14v2H7zm0 6h14v2H7zm-3 2.5c.82 0 1.5-.68 1.5-1.5s-.67-1.5-1.5-1.5-1.5.68-1.5 1.5.68 1.5 1.5 1.5z"/><circle cx="4" cy="12" r="1.5"/></svg>
      </button>
      <button @click="$emit('show-playlist')">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M0 0h24v24H0V0z" fill="none"/><circle cx="10.01" cy="17" opacity=".3" r="2"/><path d="M12 3l.01 10.55c-.59-.34-1.27-.55-2-.55C7.79 13 6 14.79 6 17s1.79 4 4.01 4S14 19.21 14 17V7h4V3h-6zm-1.99 16c-1.1 0-2-.9-2-2s.9-2 2-2 2 .9 2 2-.9 2-2 2z"/></svg>
      </button>
      <button @click="$emit('show-player')">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M12 16c-2.69 0-5.77 1.28-6 2h12c-.2-.71-3.3-2-6-2z" opacity=".3"/><circle cx="12" cy="8" opacity=".3" r="2"/><path d="M12 14c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4zm-6 4c.22-.72 3.31-2 6-2 2.7 0 5.8 1.29 6 2H6zm6-6c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0-6c1.1 0 2 .9 2 2s-.9 2-2 2-2-.9-2-2 .9-2 2-2z"/></svg>
      </button>
  </div>    
</template>

<script>
export default {
    name: 'Navigator',
}
</script>

<style lang="scss" scoped>
    .navigation{
        background-color: #202740;
        position: fixed;
        left: 0;
        bottom:0;
        height: 70px;
        width: 100%;
        display: flex;
        justify-content: space-around;
        align-items: center;
        z-index: 999;
    }
    button{
        background-color: transparent;
        border: none;
        cursor: pointer;
        -webkit-tap-highlight-color: transparent;
        outline: none;
        transition: transform .1s ease;

        svg{
            width: 50px;
            height: 50px;
            fill:#3DC864;
        }

        &:active{
            transform: scale(1.1)
        }
    }
</style>