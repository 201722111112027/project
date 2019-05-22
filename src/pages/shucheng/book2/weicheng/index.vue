<template>
  <div class="counter-warp">
    <i-panel>
    <view class="setting">
    <i-cell-group class="setting1">
    <i-cell title="前言" is-link url="/pages/shucheng/book2/mulu/qianyan/main"></i-cell>
    <i-cell title="序" is-link url="/pages/shucheng/book2/mulu/xu/main"></i-cell>
    <i-cell title="第一章" is-link url="/pages/shucheng/book2/mulu/1/main"></i-cell>
    <i-cell title="第二章" is-link url="/pages/shucheng/book2/mulu/2/main"></i-cell>
    <i-cell title="第三章" is-link url="/pages/shucheng/book2/mulu/3/main"></i-cell>
    <i-cell title="第四章" is-link url="/pages/shucheng/book2/mulu/4/main"></i-cell>
    <i-cell title="第五章" is-link url="/pages/shucheng/book2/mulu/5/main"></i-cell>
    <i-cell title="第六章" is-link url="/pages/shucheng/book2/mulu/6/main"></i-cell>
    <i-cell title="第七章" is-link url="/pages/shucheng/book2/mulu/7/main"></i-cell>
    <i-cell title="第八章" is-link url="/pages/shucheng/book2/mulu/8/main"></i-cell>
    <i-cell title="第九章" is-link url="/pages/shucheng/book2/mulu/9/main"></i-cell>
    
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
