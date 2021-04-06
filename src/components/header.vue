<template>
  <div class="header">
    <div class="header-left">
      <span class="iconfont icon-back">&#xe601;</span>
    </div>
    <div class="header-input">

      <span class="iconfont icon-search">&#xe608;</span>
      输入城市/景点/主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont icon-downselect">&#xe611;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  components: {
  }
}
</script>

<style lang='stylus' scoped>
  @import '~styles/varibles.styl'
  .header
    display: flex
    line-height: .86rem
    background: $bgColor
    color: #fff
    .header-left
      width: .64rem
      float: left
      .icon-back
        text-align: center
        font-size: .4rem
    .header-input
      flex: 1
      height: .64rem
      line-height: .64rem
      margin-top: .12rem
      margin-left: .2rem
      padding-left: .2rem
      background: #fff
      border-radius: .1rem
      color: #ccc
      .icon-search
        margin-left: .5rem
    .header-right
      width: 1.24rem
      float: right
      text-align: center
      .icon-downselect
        font-size: .24rem
        margiin-left: -.4rem
</style>
