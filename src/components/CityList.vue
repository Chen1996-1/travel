<template>
  <div class="list" ref="wrapper">
    <div>
      <div class="area">
        <div class="title border-topbottom">当前城市</div>
        <div class="button-list">
          <div class="button-swiper">
            <div class="button">北京</div>
          </div>
          <div class="button-swiper">
            <div class="button">北京</div>
          </div>
          <div class="button-swiper">
            <div class="button">北京</div>
          </div>
          <div class="button-swiper">
            <div class="button">北京</div>
          </div>
        </div>
      </div>
      <div class="area">
        <div class="title border-topbottom">热门城市</div>
        <div class="button-list">
          <div class="button-swiper">
            <div class="button">北京</div>
          </div>
          <div class="button-swiper">
            <div class="button">北京</div>
          </div>
          <div class="button-swiper">
            <div class="button">北京</div>
          </div>
          <div class="button-swiper">
            <div class="button">北京</div>
          </div>
        </div>
      </div>
      <div class="area">
        <div class="title border-topbottom">A</div>
        <div class="item-list">
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
        </div>
      </div>
      <div class="area">
        <div class="title border-topbottom">A</div>
        <div class="item-list">
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
        </div>
      </div>
      <div class="area">
        <div class="title border-topbottom">A</div>
        <div class="item-list">
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
        </div>
      </div>
      <div class="area">
        <div class="title border-topbottom">A</div>
        <div class="item-list">
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
          <div class="item border-bottom">alaer</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Bscroll from 'better-scroll'
export default {
  name: 'CityList',
  mounted () {
    this.scroll = new Bscroll(this.$refs.wrapper)
  }
}
</script>

<style lang="stylus" scoped>
@improt '~styles/varibles.styl'
.border-bottom
  &:before
    border-color: #ccc
.border-topbottom
  &:before
    border-color: #ccc
  &:after
    border-color: #ccc
.list
  width: 100%
  overflow: hidden
  position: absolute
  top: 5rem
  left: 0
  bottom: 0
  .title
    line-height: 1.5rem
    background: #eee
    padding-left: 1rem
    color: #666
  .button-list
    overflow: hidden
    padding: .5rem 4rem .5rem .5rem
    .button-swiper
      float: left
      width: 33.33%
      .button
        margin: .2rem
        padding: .3rem 0
        text-align: center
        border: .05rem solid #ccc
        border-radius: .3rem
  .item-list
    .item
      line-height: 1.5rem
      padding-left: 1rem
      color: #666
</style>
