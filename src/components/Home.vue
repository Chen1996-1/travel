<template>
  <div>
    <home-header></home-header>
    <home-swipter></home-swipter>
    <home-icons></home-icons>
  </div>
</template>

<script>
import HomeHeader from './HomeHeader.vue'
import HomeSwipter from './homeSwiper.vue'
import HomeIcons from './HomeIcons.vue'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwipter,
    HomeIcons
  }
}
</script>

<style>

</style>
