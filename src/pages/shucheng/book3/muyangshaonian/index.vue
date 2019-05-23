<template>
  <div class="counter-warp">
    <i-panel>
    <view class="setting">
    <i-cell-group class="setting1">
    <i-cell title="自序" is-link url="/pages/shucheng/book3/mulu/zixu/main"></i-cell>
    <i-cell title="第一章" is-link url="/pages/shucheng/book3/mulu/1/main"></i-cell>
    <i-cell title="第二章" is-link url="/pages/shucheng/book3/mulu/2/main"></i-cell>
    <i-cell title="第三章" is-link url="/pages/shucheng/book3/mulu/3/main"></i-cell>
    <i-cell title="第四章" is-link url="/pages/shucheng/book3/mulu/4/main"></i-cell>
    <i-cell title="第五章" is-link url="/pages/shucheng/book3/mulu/5/main"></i-cell>
    <i-cell title="第六章" is-link url="/pages/shucheng/book3/mulu/6/main"></i-cell>
    <i-cell title="第七章" is-link url="/pages/shucheng/book3/mulu/7/main"></i-cell>
    <i-cell title="第八章" is-link url="/pages/shucheng/book3/mulu/8/main"></i-cell>
    <i-cell title="第九章" is-link url="/pages/shucheng/book3/mulu/9/main"></i-cell>
    <i-cell title="第十章" is-link url="/pages/shucheng/book3/mulu/10/main"></i-cell>
    <i-cell title="第十一章" is-link url="/pages/shucheng/book3/mulu/11/main"></i-cell>
    <i-cell title="第十二章" is-link url="/pages/shucheng/book3/mulu/12/main"></i-cell>
    <i-cell title="第十三章" is-link url="/pages/shucheng/book3/mulu/13/main"></i-cell>
    <i-cell title="第十四章" is-link url="/pages/shucheng/book3/mulu/14/main"></i-cell>
    <i-cell title="第十五章" is-link url="/pages/shucheng/book3/mulu/15/main"></i-cell>
    <i-cell title="第十六章" is-link url="/pages/shucheng/book3/mulu/16/main"></i-cell>
     <i-cell title="第十七章" is-link url="/pages/shucheng/book3/mulu/17/main"></i-cell>
    <i-cell title="第十八章" is-link url="/pages/shucheng/book3/mulu/18/main"></i-cell>
     <i-cell title="第十九章" is-link url="/pages/shucheng/book3/mulu/19/main"></i-cell>
    <i-cell title="第二十章" is-link url="/pages/shucheng/book3/mulu/20/main"></i-cell>
     <i-cell title="第二十一章" is-link url="/pages/shucheng/book3/mulu/21/main"></i-cell>
    
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
