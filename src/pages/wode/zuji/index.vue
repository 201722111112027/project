<template>
  <div class="counter-warp">
    <i-panel>
    <view class="setting">
    <i-cell-group class="setting1">
    <i-cell title="平凡世界" is-link url="/pages/book1/index/main"></i-cell>
    <i-cell title="围城" is-link url="/pages/book2/index/main"></i-cell>
    <i-cell title="人间失格" is-link url="/pages/book4/index/main"></i-cell>
    <i-cell title="武动乾坤" is-link url="/pages/shujia/wudong/main"></i-cell>
    <i-cell title="三生三世十里桃花" is-link url="/pages/shujia/shilitaohua/main"></i-cell>
    <i-cell title="三生三世枕上书" is-link url="/pages/shujia/zhenshangshu/main"></i-cell>
    <i-cell title="大主宰" is-link url="/pages/shujia/dazhuzai/main"></i-cell>
    <i-cell title="斗破苍穹" is-link url="/pages/shujia/doupo/main"></i-cell>
    <i-cell title="修仙万年归来" is-link url="/pages/shujia/doupo/main"></i-cell>
    <i-cell title="帝都风云" is-link url="/pages/shujia/doupo/main"></i-cell>
    <i-cell title="我不喜欢这世界，我只喜欢你" is-link url="/pages/shujia/doupo/main"></i-cell>
    </i-cell-group>
    </view>
    </i-panel>
  </div>
</template>

<script>
// Use Vuex
import store from './store'

export default {
  computed: {
    data () {
      return {
      } 
    },
   
  }
}
</script>

<style>
.counter-warp {
  margin-top: 2px;
  
}
.setting1{
  background-color:	Peru
}
.home {
  display: inline-block;
  margin: 100px auto;
  padding: 5px 10px;
  color: blue;
  border: 1px solid blue;
}
</style>
