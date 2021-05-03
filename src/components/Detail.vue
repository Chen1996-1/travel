<template>
 <div>
   <detail-banner></detail-banner>
   <detail-header></detail-header>
   <detail-list :list="categoryList"></detail-list>
   <div class="test-height"></div>
 </div>
</template>

<script>
import DetailBanner from './DetailBanner.vue'
import DetailHeader from './DetailHeader.vue'
import DetailList from './DetailList.vue'

export default {
  name: 'Detail',
  components: {
    DetailBanner,
    DetailHeader,
    DetailList
  },
  data () {
    return {
      categoryList: [{
        title: '成人票',
        children: [{
          title: '成人三馆联票',
          children: [{
            title: '成人三馆联票 - 某一连锁店销售'
          }]
        }, {
          title: '成人五馆联票'
        }]
      }, {
        title: '学生票'
      }, {
        title: '儿童票'
      }, {
        title: '特惠票'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
.test-height
  height: 1000rem

</style>
