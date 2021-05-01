<template>
  <div>
    <div class="banner" @click="handleClickGallaryImgs">
      <img class="banner-img" src="http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_600x330_bf9c4904.jpg"/>
      <div class="banner-info">
        <div class="info-title">
          兴义海洋馆
        </div>
        <div class="info-counts">
          <span class="iconfont icon-img">&#xe6df;</span>
        34
        </div>
      </div>
    </div>
    <common-gallary :list="gallaryImgs" v-show="showGallary" @handleClickBackBanner="handleClickBackBanner"></common-gallary>
  </div>
</template>

<script>
import CommonGallary from './CommonGallary.vue'
export default {
  name: 'DetailBanner',
  components: { CommonGallary },
  data () {
    return {
      showGallary: false,
      gallaryImgs: ['http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_800x800_70debc93.jpg', 'http://img1.qunarzz.com/sight/p0/1709/76/7691528bc7d7ad3ca3.img.png_800x800_9ef05ee7.png']
    }
  },
  methods: {
    handleClickGallaryImgs () {
      this.showGallary = true
    },
    handleClickBackBanner () {
      this.showGallary = false
    }
  }
}
</script>

<style lang="stylus" scoped>
.banner
  position: relative
  overflow: hidden
  height: 0
  padding-bottom: 55%
  .banner-img
    width: 100%
  .banner-info
    display: flex
    position: absolute
    left: 0
    right: 0
    bottom: 0
    height: 1.5rem
    line-height: 1.5rem
    background-image: linear-gradient(top, rgba(0,0,0,0), rgba(0,0,0,0.8))
    color: #fff
    .info-title
      flex: 1
      padding-left: 1rem
    .info-counts
      padding: .5rem
      height: .8rem
      line-height: .8rem
      border-radius: .2rem
      background: rgba(0,0,0,.2)
      .icon-img
        color: #fff
        font: .8rem
</style>
