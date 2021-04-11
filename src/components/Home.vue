<template>
  <div>
    <home-header></home-header>
    <home-swipter></home-swipter>
    <home-icons></home-icons>
    <home-recommand></home-recommand>
    <home-weekend></home-weekend>
  </div>
</template>

<script>
import HomeHeader from './HomeHeader.vue'
import HomeSwipter from './homeSwiper.vue'
import HomeIcons from './HomeIcons.vue'
import HomeRecommand from './HomeRecommand.vue'
import HomeWeekend from './HomeWeekend.vue'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwipter,
    HomeIcons,
    HomeRecommand,
    HomeWeekend
  }
}
</script>

<style>

</style>
