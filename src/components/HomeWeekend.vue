<template>
  <div>
    <div class="weekend-block-title">周末去哪玩</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl"/>
        </div>
        <div class="item-info-wrapper">
          <p class="item-info-title">{{item.title}}</p>
          <p class="item-info-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
        id: '00001',
        imgUrl: 'https://tse1-mm.cn.bing.net/th?id=OIP.MEWCmUbayAoQ-NpLUVFBCwHaEK&w=305&h=160&c=8&rs=1&qlt=90&dpr=1.25&pid=3.1&rm=2',
        title: '推荐一',
        desc: '巴拉巴拉巴拉巴'
      },
      {
        id: '00002',
        imgUrl: 'https://tse1-mm.cn.bing.net/th?id=OIP.MEWCmUbayAoQ-NpLUVFBCwHaEK&w=305&h=160&c=8&rs=1&qlt=90&dpr=1.25&pid=3.1&rm=2',
        title: '推荐一',
        desc: 'bbaladfjsdfjkasdfjkasd'
      },
      {
        id: '00003',
        imgUrl: 'https://tse1-mm.cn.bing.net/th?id=OIP.MEWCmUbayAoQ-NpLUVFBCwHaEK&w=305&h=160&c=8&rs=1&qlt=90&dpr=1.25&pid=3.1&rm=2',
        title: '推荐一',
        desc: 'ajdfkasjdfkasjdf'
      }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl'
 .weekend-block-title
    margin-top: 1rem
    line-height: 1.8rem
    background: #eee
    text-indent: 1rem
  .item-info-wrapper
    overflow: hidden
    height: 0
    padding-bottom: 4rem
    .item-img
      width:100%
    .item-info-title
      line-height: 1.5rem
      ellipsis()
    .item-info-desc
      line-height: 1rem
      color: #ccc
      ellipsis()
</style>
