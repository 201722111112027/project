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
    <i-panel class="panel">
    <text class="text"> 寻遍三生兜兜转转，灼灼桃林之下，还是只想与你执手死生契阔 
不如，你便以身相许吧
——三生三世十里桃花《三生三世十里桃花》</text>
    </i-panel>
   <i-grid i-class="no-border">
    <i-grid-item @click="start" class="test">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1557854121615&di=b6b001204cc993e8bd6684863bf2dd86&imgtype=0&src=http%3A%2F%2Fpic.51yuansu.com%2Fpic2%2Fcover%2F00%2F32%2F00%2F5810d7724ac54_610.jpg" />
        </i-grid-icon>
        <i-grid-label  >免费试读</i-grid-label>
    </i-grid-item>
     <i-grid-item @click="start" i-class="no-border">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1557854373039&di=3f1b9e375b73757c545add8fc9e40a03&imgtype=0&src=http%3A%2F%2Fpic.51yuansu.com%2Fpic2%2Fcover%2F00%2F35%2F45%2F5811a08bbb569_610.jpg" />
        </i-grid-icon>
        <i-grid-label>全本下载</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="logisiticsGZFn" i-class="no-border">
        <i-grid-icon>
            <image src="http://pic.51yuansu.com/pic2/cover/00/32/93/58110d765aa63_610.jpg" />
        </i-grid-icon>
        <i-grid-label>加入书架</i-grid-label>
    </i-grid-item>
    </i-grid> 
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
        'http://img0.imgtn.bdimg.com/it/u=3242313580,2727575826&fm=26&gp=0.jpg',
        'http://img5.imgtn.bdimg.com/it/u=903521236,2408838169&fm=26&gp=0.jpg',
        'http://img4.imgtn.bdimg.com/it/u=3208662069,1201475381&fm=26&gp=0.jpg',
        'http://img5.imgtn.bdimg.com/it/u=2566856047,3867072578&fm=26&gp=0.jpg',
        'http://img3.imgtn.bdimg.com/it/u=3449894133,4223329732&fm=26&gp=0.jpg',
        'http://img1.imgtn.bdimg.com/it/u=936444481,1837250808&fm=26&gp=0.jpg',
        'http://img3.imgtn.bdimg.com/it/u=105972846,3132699987&fm=26&gp=0.jpg'
      ],
      indicatorDots: false,
      autoplay: true,
      interval: 5000,
      duration: 1000
    }
  },
  methods: {
    // start(){
    //   wx.navigateTo({
    //     url: '/pages/book1/pfsj/main'
    //   })
    // },
    
    logisiticsGZFn(){
      wx.showToast({
      title: '成功添加',
      icon: 'success',
      duration: 2000
      })
    }
  }
}
</script>

<style scoped>
div >>>.no-boder{
  border-width: 0pt;
  background-color: brown;
  height: 20px;
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

.test{
   background-color:red
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
  height:240rpx;
  text-indent: 2em;
}


p {text-indent: 2em;}
.panel{
  color:Orange;
  text-indent:5em;
   margin-top:0pt;
   width:580rpx;
   height:240rpx;
   text-indent: 2em;
}
</style>
