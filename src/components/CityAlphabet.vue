<template>
  <div class="alphabet-list">
    <ul class="list">
      <li class="item">A</li>
      <li class="item">A</li>
      <li class="item">A</li>
      <li class="item">A</li>
      <li class="item">A</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'CityAlphabet'
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.list
  display: flex
  flex-direction: column
  justify-content: center
  position: absolute
  right:0
  bottom:0
  top: 5rem
  width: 2rem
  .item
    line-height: 1.5rem
    text-align: right
    color: $bgColor
</style>
