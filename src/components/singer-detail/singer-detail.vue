<template>
  <transition name="slider">
    <div class="singer-detail"></div>
  </transition>
</template>

<script>
  export default {
    data() {
      return {

      }
    }
  }
</script>

<style scoped lang="stylus">
  @import "~common/stylus/variable"

  .singer-detail
    position: fixed
    z-index: 100
    top: 0
    left: 0
    right: 0
    bottom: 0
    background: $color-background

  .slider-enter-active, .slide-leave-active
    transition: all 0.3s

  .slider-enter, .slider-leave-to
    transform: translate3d(100%, 0, 0)

</style>
