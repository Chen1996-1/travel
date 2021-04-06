<template>
<div class="wrapper">
  <swiper :options="swiperOptions">
    <swiper-slide v-for="img of swiperList" :key="img.id">
      <img class="img-swiper" :src="img.imgUrl">
    </swiper-slide>
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
</div>
</template>

<script>
export default {
  name: 'HomeSwipter',
  data: function () {
    return {
      swiperOptions: {
        pagination: '.swiper-pagination'
        // Some Swiper option/callback...
      },
      swiperList:
      [
        {
          id: '001',
          imgUrl: 'https://s.cn.bing.net/th?id=ABT1858A5CC2F977FDB056C766960B4FE2153F2E4E6B2E5A6BD8E24537757FD1059&w=608&h=200&c=2&rs=1&dpr=1.25&pid=SANGAM'
        },
        {
          id: '002',
          imgUrl: 'https://s.cn.bing.net/th?id=ABTBA338AD926E4968FAC7A68658F8BE1843F478003D90DBE27839FBE02595CBE60&w=608&h=200&c=2&rs=1&dpr=1.25&pid=SANGAM'
        },
        {
          id: '003',
          imgUrl: 'https://www.bing.com/th/id/ABTFFC8C4BD50BD24A57442916ADF2D52F52A750E4031575E778AF113C0215BA393?qlt=90&dpr=1.25&pid=InlineBlock'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background: #fff
  .wrapper
    width:100%
    height:0
    padding-bottom:31.25%
  .img-swiper
    width: 100%

</style>
