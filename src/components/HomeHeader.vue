<template>
  <div class="header">
    <div class="header-left">
      <span class="iconfont icon-back">&#xe601;</span>
    </div>
    <div class="header-center">

      <span class="iconfont icon-search">&#xe608;</span>
      输入城市/景点/主题
    </div>
    <div class="header-right">
      {{city}}
      <span class="iconfont icon-downselect">&#xe611;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang='stylus' scoped>
  @import '~styles/varibles.styl'
  .header
    background:$bgColor
    display: flex
    height: 2.5rem
    line-height: 2.5rem

    .header-left
      margin-left: 1rem
      margin-right: 1.5rem
      .icon-back
        font-size: 1.3rem
    .header-center
      margin-right: 1rem
      background: #fff
      border-radius: .25rem
      margin-top: .15rem
      margin-bottom: .25rem
      padding-left: .8rem
      padding-right:3rem
      color: #ccc
    .header-right
      text-align: center
      .icon-downselect
        font-size: .8rem
        padding-left: .2rem

</style>
