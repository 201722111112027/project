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
    <text class="text">我现在很快乐，我没有特别自卑了，我的生活轻松愉悦，每天都努力让自己变得更好，我去参加社团学生会各种选修课，一点一点变优秀，我对未来充满期许。现在的我是最好的我，如果你在我身边就好了。

　　只是春光如此，却不得见你。——《我只喜欢你》</text>
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
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559313913978&di=f3f48a7233d3fde09f010c750402d6f7&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201608%2F15%2F20160815232945_nhJfa.thumb.700_0.jpeg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559313913977&di=9768af63dee3c81c0f4c1beeb74a1c82&imgtype=0&src=http%3A%2F%2Fhbimg.b0.upaiyun.com%2F5166d34a255284fe197d48c1614de6783abd291832f6e-FrQ518_fw658',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559313913975&di=9c7718f0560da9c4949f0c6b681509c7&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201802%2F12%2F20180212113648_bpdwf.thumb.700_0.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559313913974&di=3829d6027383250954eccf517a898169&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201608%2F15%2F20160815233245_VTcQn.thumb.700_0.jpeg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559313913972&di=6666b3bbbbdfb813692175d726eba338&imgtype=0&src=http%3A%2F%2Fimg3.duitang.com%2Fuploads%2Fitem%2F201608%2F16%2F20160816015419_xQZCy.thumb.700_0.jpeg',
        
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
