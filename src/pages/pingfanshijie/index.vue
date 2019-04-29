<template>
  <div class="counter-warp">
    <i-panel><view class="setting" bindtap='jumpLogin'>
      <image class="image1" src='http://img1.imgtn.bdimg.com/it/u=929659737,3108829528&fm=15&gp=0.jpg' style="width:130rpx;height:180rpx;"></image>   
        <text style="padding:7px;line-height:17px">
      <text class="first">《平凡的世界》是中国作家路遥创作的一部百万字的小说。这是一部全景式地表现中国当代城乡社会生活的长篇小说，全书共三部。1986年12月首次出版。</text>
   </text>
   </view>
    </i-panel>
  </div>
</template>

<script>
// Use Vuex
import store from './store'

export default {
  
}
</script>

<style scoped>
div >>>.no-boder{
  border-width: 0pt;
}
.setting{
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-left: 9px;
  margin-top: 5px;
}
.top-padding{
  padding-top:20rpx;
}
.first{
  color:black;
  font-size: 40rpx;
  font-family: microsoft yahei;
  font-weight: normal;
  letter-spacing: 1.5px;
}
.second{
  color:black;
  font-size: 40rpx;
  font-family: microsoft yahei;
  font-weight: normal;
  letter-spacing: 1.5px;
}
.third{
  color:black;
  font-size: 40rpx;
  font-family: microsoft yahei;
  font-weight: normal;
  letter-spacing: 1.5px;
}
.forth{
  color:black;
  font-size: 40rpx;
  font-family: microsoft yahei;
  font-weight: normal;
  letter-spacing: 1.5px;
}
.fivth{
  color:black;
  font-size: 40rpx;
  font-family: microsoft yahei;
  font-weight: normal;
  letter-spacing: 1.5px;
}
.sixth{
  color:black;
  font-size: 40rpx;
  font-family: microsoft yahei;
  font-weight: normal;
  letter-spacing: 1.5px;
}
.image1{
  
}
</style>
