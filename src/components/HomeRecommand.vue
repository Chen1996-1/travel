<template>
  <div>
    <div class="recommend-block-title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl"/>
        </div>
        <div class="item-info-wrapper">
          <p class="item-info-title">{{item.title}}</p>
          <p class="item-info-desc">{{item.desc}}</p>
          <button class="item-info-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommand',
  data () {
    return {
      recommendList: [{
        id: '00001',
        imgUrl: 'https://s.cn.bing.net/th?id=ABTA8911B5D0EB388D4AAA3E9831AD0E2EC02EB48A48833CE7A71381CB3CB86ABAA&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM',
        title: '推荐一',
        desc: '巴拉巴拉巴拉巴'
      },
      {
        id: '00002',
        imgUrl: 'https://s.cn.bing.net/th?id=ABTA8911B5D0EB388D4AAA3E9831AD0E2EC02EB48A48833CE7A71381CB3CB86ABAA&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM',
        title: '推荐一',
        desc: 'bbaladfjsdfjkasdfjkasd'
      },
      {
        id: '00003',
        imgUrl: 'https://s.cn.bing.net/th?id=ABTA8911B5D0EB388D4AAA3E9831AD0E2EC02EB48A48833CE7A71381CB3CB86ABAA&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM',
        title: '推荐一',
        desc: 'ajdfkasjdfkasjdf'
      },
      {
        id: '00004',
        imgUrl: 'https://s.cn.bing.net/th?id=ABTA8911B5D0EB388D4AAA3E9831AD0E2EC02EB48A48833CE7A71381CB3CB86ABAA&w=120&h=120&c=1&rs=1&qlt=80&dpr=1.25&pid=SANGAM',
        title: '推荐一',
        desc: 'asdfjaskdfjaskdjfklasdjfasdjfkasdjfias'
      }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl'
 .recommend-block-title
    margin-top: 1rem
    line-height: 1.8rem
    background: #eee
    text-indent: 1rem
  .item
    display: flex
    height: 5rem
    .item-img
      width: 4rem
      height: 4rem
      padding:.5rem
    .item-info-wrapper
      flex: 1
      padding: .2rem
      min-width: 0
      .item-info-title
        line-height: 1.5rem
        ellipsis()
      .item-info-desc
        line-height: 1rem
        color: #ccc
        ellipsis()
      .item-info-button
        line-height: 1.2rem
        margin-top: .3rem
        background: #ff9300
        padding: 0 .2rem
        border-radius: .3rem
        collor: #fff

</style>
