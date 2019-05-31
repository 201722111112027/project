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
    <i-panel class="panel">
    <text class="text"> 留下是希望可以每天看着你的笑，如果这不是你想要的，如果这样会让你有一丝丝难受，就不是我的本意了，你有这么大的胸襟放我去飞，我何尝没有这么大的胸襟为你去飞？我能为你留，当然也能为你走。

—— 赵乾乾</text>
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
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314338246&di=cf0810c671f41fc68389be9215a630aa&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201608%2F19%2F20160819092621_cPhns.thumb.700_0.jpeg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314338245&di=952a1a667be4476f4267030fdbde0e55&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201609%2F11%2F20160911094358_2X4MS.jpeg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314338245&di=4a40274d7da2bc96693ad394ef8c49f6&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201509%2F17%2F20150917200549_hz3wc.jpeg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314338245&di=d54fcddd49b913dbf16b5f7d98178f45&imgtype=0&src=http%3A%2F%2Fimg3.duitang.com%2Fuploads%2Fitem%2F201509%2F19%2F20150919210729_FJXmx.jpeg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314338244&di=f41a1d45defa0d402997519d04951503&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201609%2F04%2F20160904161601_kLzvY.jpeg',
        
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
