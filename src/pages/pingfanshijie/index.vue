<template>
  <div class="counter-warp">
    <swiper
      :indicator-dots="indicatorDots"
      :autoplay="autoplay"
      :interval="interval"
      :duration="duration"
      style="height:240px"
    >
    <block v-for="item in imgUrls" :key="item">
      <swiper-item>
        <image :src="item" style="width:100%;"/>
      </swiper-item>
    </block>
  </swiper>
    <!-- <i-panel><view class="setting" bindtap='jumpLogin'>
      <image class="image1" src='http://img1.imgtn.bdimg.com/it/u=929659737,3108829528&fm=15&gp=0.jpg' style="width:130rpx;height:180rpx;"></image>   
      <text class="text" style="padding:7px;line-height:17px">
      <text class="first">《平凡世界》\n</text>
      <text class="sceond">路遥|史诗巨作\n\n</text>
      <text class="third">9.7分</text>
   </text>
   </view>
    </i-panel> -->
    <i-panel><view class="pingfen">
      <i-rate 
            :change="onChange2" 
            value="starIndex2"
            size="32">评分
        </i-rate>
        <!-- <text class="renqi">2867.1万</text>
        <text class="fensi">77万</text> -->
        </view>
    </i-panel>
    <i-panel >
    <text class="text">  青年，青年！无论受怎样的挫折和打击，都要咬着牙冠挺住，因为你们完全有机会重建生活；只要不灰心丧气，每一次挫折，只不过是通往新境界的一块普通绊脚石而绝不会置人于死命。                         ——路遥</text>
    </i-panel>
    
  <i-cell-group>
    <i-cell title="目录  20章" is-link url="/pages/pfsj/main"></i-cell>
</i-cell-group>
<i-panel>
  <view class="button">
<button @click="handleClick" type="primary" style="color:red" >加入书架</button>
</view>
</i-panel>
  </div>
</template>

<script>
// Use Vuex
import store from './store'

export default {
  data () {
    return {
     starIndex2 : 4.5,
     imgUrls:[
        'http://img1.imgtn.bdimg.com/it/u=2049799998,1577767969&fm=26&gp=0.jpg',
        'http://img0.imgtn.bdimg.com/it/u=2057511425,2529990695&fm=26&gp=0.jpg',
        'http://img5.imgtn.bdimg.com/it/u=1726489621,789915892&fm=26&gp=0.jpg',
        'http://img1.imgtn.bdimg.com/it/u=1145045993,3394112898&fm=11&gp=0.jpg',
        'http://img2.imgtn.bdimg.com/it/u=3211702520,2203896700&fm=26&gp=0.jpg',
        'http://img2.imgtn.bdimg.com/it/u=2937290376,1303931150&fm=11&gp=0.jpg',
        'http://img1.imgtn.bdimg.com/it/u=2975002125,4179887462&fm=26&gp=0.jpg'
      ],
      indicatorDots: false,
      autoplay: true,
      interval: 5000,
      duration: 1000
    }
  },
  methods: {
    onChange2(e){
        const index = e.detail.index;
        this.setData({
            'starIndex2' : index
        })
    },
    handleClick(){
       
    }
  }
}
</script>

<style scoped>
div >>>.no-boder{
  border-width: 0pt;
}
.setting{
  background-color:	DarkKhaki;
  width:100%;
  height:200px;
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-left: 0px;
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
  row-spacing:2px;
   margin-left: 40px;
   margin-top: 5px;
}
.sceond{
  color:Orange;
  font-size: 40rpx;
  font-family: microsoft yahei;
  font-weight: normal;
  letter-spacing: 1.5px;
   margin-left: 40px;
  margin-top: 5px;
}
.third{
  color:black;
  font-size: 40rpx;
  font-family: microsoft yahei;
  font-weight: normal;
  letter-spacing: 3px;
   margin-left: 40px;
   margin-top: 5px;
}
.image1{
  width:180px;
  height:150px;
   margin-top:10rpx;
   margin-left:10rpx;
}
.text{
  color:Orange;
  text-indent:5em;
   margin-top:0pt;
   width:580rpx;
   height:120rpx;
   text-indent: 2em
}
.mulu{
  color:GoldEnrod;
  width:100%;
  height:30px;
}
.button{
  background-color:red;
}
</style>
