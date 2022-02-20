<template>
  <button class="rate-btn" 
    :class="{
      'rate-btn--like': isLike,
      'rate-btn--hate': !isLike,  
    }"
  >
    <slot/>
  </button>
</template>

<script>
export default {
  name: 'LikeBtn',
  props: {
    isLike: {
      type: Boolean,
      default: true,
    }
  },
  data() {
    return{
    }
  }
}
</script>

<style lang="scss" scoped>
.rate-btn{
  background: transparent;
  border:none;
  text-align: center;
  line-height: 0.5;
  cursor: pointer;
  text-align: center;
  font-size: 16px;
  border-radius: 50px;
  padding: 5px;

  &--like{
      border: 2px solid #127012;
      color: #127012;
  }
  &--hate{
      border: 2px solid red;
      color: red;
  }
}
</style>