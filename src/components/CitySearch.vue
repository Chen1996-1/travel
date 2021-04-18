<template>
  <div class="search">
    <input class="search-input" type="text" placeholder="输入城市名或拼音">
  </div>
</template>

<script>
export default {
  name: 'CitySearch'
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.search
  height: 2.5rem
  padding: 0 .5rem
  background: $bgColor
  .search-input
    box-sizing: border-box
    width: 100%
    height: 2rem
    line-height: 2rem
    padding: 0 .5rem
    text-align: center
    border-radius: .3rem
    color: #667
</style>
