<template>
<swiper>
  <swiper-slide v-for="(iconList,index) of pageProjects" :key="index">
  <div class="icons">
    <div class="icon" v-for="iconItem of iconList" :key="iconItem.content">
      <div class="icon-img">
        <img class="icon-img-img" :src="iconItem.iconImgUrl">
      </div>
      <div class="icon-content">
        {{ iconItem.content}}
      </div>
    </div>
  </div>
  </swiper-slide>
</swiper>
</template>

<script>
export default {
  name: 'HomeIcons',
  data () {
    return {
      iconList: [
        {content: '1七彩宝石wocccccccccccccc', iconImgUrl: 'https://s.cn.bing.net/th?id=ABT7948A0210AF99F812051D7DE1818EEEB53022641C79BA1B41D86BF6A0C3182F7&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM'},
        {content: '2州立公园', iconImgUrl: 'https://s.cn.bing.net/th?id=ABTA8913B5D0EB388D4AAA3E9831AD0E2EC02EB48A48833CE7A71381CB3CB86ABAA&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM'},
        {content: '3变色湖泊', iconImgUrl: 'https://s.cn.bing.net/th?id=ABT465641A2F542B4438F8DC711081940F06B299EFB2111E6DAE7F0DE771E939F3C&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM'},
        {content: '4波俄图', iconImgUrl: 'https://s.cn.bing.net/th?id=ABT9FD4AA0B67ECCDA2FEF2C0CB5B442863D93EF52CC679EE32745A3021194DB7B6&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM'},
        {content: '5野大白羊', iconImgUrl: 'https://s.cn.bing.net/th?id=ABT6C5482F3FCEB4D992E849284BE5C8131EEA1636D5FCD45927C9205F060A7FD72&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM'},
        {content: '6布列塔尼', iconImgUrl: 'https://s.cn.bing.net/th?id=ABT3CACA88EA5BB85F9C669551CEACA90CE04936506D7348E18B4F10E5EC005745E&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM'},
        {content: '7西雅图', iconImgUrl: 'https://s.cn.bing.net/th?id=ABT50CD26BEBBEA09483B47C473A5E78F74B2A4B8EDE7A74D9E2BE934A4C013B778&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM'},
        {content: '8tttt', iconImgUrl: 'https://s.cn.bing.net/th?id=ABT267602ABB5236016CC958316145F598BE4D958DED9F984F1223CBD359ADA0E88&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM'},
        {content: '9坤图兰', iconImgUrl: 'https://s.cn.bing.net/th?id=ABT2AE90F9C7D6B915E40157F8022D01A32A13E01582C48D6655B602B9C20470BFF&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM'},
        {content: '10Drangarnir', iconImgUrl: 'https://s.cn.bing.net/th?id=ABT9C92D08814F755ECDC513840573288BD007BBE6585A3EF5292AB3206413CFD08&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM'}
      ]
    }
  },
  computed: {
    pageProjects () {
      const pageProjects = []
      this.iconList.forEach((item, index) => {
        const page = Math.floor(index / 8)
        if (!pageProjects[page]) {
          pageProjects[page] = []
        }
        pageProjects[page].push(item)
      })
      return pageProjects
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl'
.icons >>> .swiper-container
.icons
  overflow : hidden
  height:0
  padding-bottom:50%
  .icon
    position: relative
    overflow: hidden
    float: left
    width: 25%
    height: 0
    padding-bottom:25%
    .icon-img
      position: absolute
      top: 0
      left: 0
      right: 0
      bottom: .44rem
      box-sizing: border-box
      padding: 1rem

      .icon-img-img
        display: block
        margin: 0 auto
        height: 100%
    .icon-content
      position: absolute
      bottom: 0
      left:0
      right:0
      text-align: center
      ellipsis()

</style>
