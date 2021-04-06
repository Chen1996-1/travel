<template>
  <div>
    <home-header></home-header>
    <home-swipter></home-swipter>
  </div>
</template>

<script>
import HomeHeader from './header.vue'
import HomeSwipter from './swiper.vue'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwipter
  }
}
</script>

<style>

</style>
