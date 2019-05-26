<template>
  <div class="counter-warp">
    <i-panel>
    <view class="setting">
    <i-cell-group class="setting1">
    <i-cell title="鱼服记" is-link url="/pages/book4/mulu/kaishi/main"></i-cell>
    <i-cell title="手记之一" is-link url="/pages/book4/mulu/zhiyi/main"></i-cell>
    <i-cell title="手记之二" is-link url="/pages/book4/mulu/zhier/main"></i-cell>
    <i-cell title="手记之三" is-link url="/pages/book4/mulu/zhisan/main"></i-cell>
    <i-cell title="后记" is-link url="/pages/book4/mulu/houji/main"></i-cell>
  
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
