<template>
  <div class="counter-warp">
    <i-panel>
    <view class="setting">
      <p>我的文化山河</p>
    <i-cell-group class="setting1">
    <i-cell title="第一章" is-link url="/pages/book5/mulu/1/main"></i-cell>
    <i-cell title="第二章" is-link url="/pages/book5/mulu/2/main"></i-cell>
    <i-cell title="第三章" is-link url="/pages/book5/mulu/3/main"></i-cell>
    <i-cell title="第四章" is-link url="/pages/book5/mulu/4/main"></i-cell>
    <i-cell title="第五章" is-link url="/pages/book5/mulu/5/main"></i-cell>
    <i-cell title="第六章" is-link url="/pages/book5/mulu/6/main"></i-cell>
    <i-cell title="第七章" is-link url="/pages/book5/mulu/7/main"></i-cell>
    <i-cell title="第八章" is-link url="/pages/book5/mulu/8/main"></i-cell>
    <p>蚩尤的后代</p>
    <i-cell title="第一章" is-link url="/pages/book5/mulu/9/main"></i-cell>
    <i-cell title="第二章" is-link url="/pages/book5/mulu/10/main"></i-cell>
    <i-cell title="第三章" is-link url="/pages/book5/mulu/11/main"></i-cell>
    <i-cell title="第四章" is-link url="/pages/book5/mulu/12/main"></i-cell>
    <i-cell title="第五章" is-link url="/pages/book5/mulu/13/main"></i-cell>
    <i-cell title="第六章" is-link url="/pages/book5/mulu/14/main"></i-cell>
    <p>我本是树</p>
    <i-cell title="第一章" is-link url="/pages/book5/mulu/15/main"></i-cell>
    <i-cell title="第二章" is-link url="/pages/book5/mulu/16/main"></i-cell>
    <i-cell title="第三章" is-link url="/pages/book5/mulu/17/main"></i-cell>
   <p>西域喀什</p>
    <i-cell title="第一章" is-link url="/pages/book5/mulu/18/main"></i-cell>
    <i-cell title="第二章" is-link url="/pages/book5/mulu/19/main"></i-cell>
    <i-cell title="第三章" is-link url="/pages/book5/mulu/20/main"></i-cell>
    <i-cell title="第四章" is-link url="/pages/book5/mulu/21/main"></i-cell>
    
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
p {size: 50px;}
</style>
