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
    <text class="text">江辰，他们说比喜欢多一点是爱，比爱多一点呢？是只爱，那比只爱多一点呢？，是不能失去，比不能失去再多一点呢，是另一个自己，比另一个自己再多一点呢，是你。————《致我们单纯的小美好》</text>
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
    <i-grid-item @click="logisiticsGZFn" i-class="no-border">
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
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559908805&di=685deb94a8c3ca23410be200c519d010&imgtype=jpg&er=1&src=http%3A%2F%2Fhbimg.b0.upaiyun.com%2Fe56e2c94bd8d28a6c6a8fdcc4d9b4b6e59796e20122d12-FUd2JS_fw658',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314129204&di=f39c14181bb59eaca7f1f3af0f48c4ec&imgtype=0&src=http%3A%2F%2Fs15.sinaimg.cn%2Fbmiddle%2F006PK9Kfzy7guRXL5Qace%26690',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314129203&di=98ba333405cf29c649c7135d2d63042e&imgtype=0&src=http%3A%2F%2Fn.sinaimg.cn%2Fsinacn%2Fw640h503%2F20171229%2F6cac-fypyuve1919750.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314129203&di=18080cf830bb550a5f116e5c27a117ab&imgtype=0&src=http%3A%2F%2Fn.sinaimg.cn%2Fsinacn%2F20171124%2Fcaa1-fypceiq1012856.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314129202&di=fde61dbe2a225c6b778308b06f9d7a9a&imgtype=0&src=http%3A%2F%2Fn.sinaimg.cn%2Ffront%2F262%2Fw640h422%2F20190109%2FaDYJ-hrkkweh2149050.jpg',
        
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
    start(){
      wx.navigateTo({
        url: '/pages/book2/weicheng/main'
      })
    },
    logisiticsGZFn(){
      $Toast({
            content: '成功的提示',
            type: 'success'
        });
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
