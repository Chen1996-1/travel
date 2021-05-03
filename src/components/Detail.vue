<template>
 <div>
   <detail-banner></detail-banner>
   <detail-header></detail-header>
   <div class="test-height"></div>
 </div>
</template>

<script>
import DetailBanner from './DetailBanner.vue'
import DetailHeader from './DetailHeader.vue'

export default {
  name: 'Detail',
  components: {
    DetailBanner,
    DetailHeader
  }
}
</script>

<style lang="stylus" scoped>
.test-height
  height: 1000rem

</style>
