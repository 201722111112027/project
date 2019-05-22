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
    <text class="text">早晨，我睁眼醒来翻身下床，又变成了原来那个浅薄无知、善于伪装的滑稽角色。胆小鬼连幸福都会惧怕，碰到棉花都会受伤，有时也会被幸福所伤。趁着还没有受伤，我想就这样赶快分道扬镳。我又放出了惯用的逗笑烟幕弹。   ————太宰治</text>
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
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="http://pic.51yuansu.com/pic2/cover/00/32/93/58110d765aa63_610.jpg" />
        </i-grid-icon>
        <i-grid-label>加入书架</i-grid-label>
    </i-grid-item>
    </i-grid> 
  <!-- <i-cell-group>
    <i-cell title="目录  20章" is-link url="/pages/book1/pfsj/main"></i-cell>
</i-cell-group>
<i-panel>
  <view class="button">
<button @click="handleClick" type="primary" style="color:red" >加入书架</button>
</view>
</i-panel> -->
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
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558503280515&di=cb6a6ee9be8085a0145952c3f38a4668&imgtype=0&src=http%3A%2F%2F02imgmini.eastday.com%2Fmobile%2F20190325%2F2019032516_a27fa8781b46481e911f440d08fc1091_8554_cover_mwpm_03201609.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558503281689&di=a66dfb57c56cf163f3e8b3ed901bc794&imgtype=0&src=http%3A%2F%2Fs8.sinaimg.cn%2Fmw690%2F0066wqsGzy76vBLCrbh07%26690',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558503281685&di=5a83e17e7c3683a8d0376ee62d624996&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201709%2F30%2F20170930152457_eUtji.thumb.700_0.jpeg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558503369651&di=076bbdd74676127220082ca36b3f0084&imgtype=0&src=http%3A%2F%2Fmmbiz.qpic.cn%2Fmmbiz_jpg%2FDCUA7Libl5wOZoXTWP8nuyu87cqrpgsDSzre9UOS2z59vdEXhgoKqzM07abZfaibzVKTic9ibMjvkxvCyI7YqD5TBA%2F640%3Fwx_fmt%3Djpeg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559098087&di=78c6b300160969ad43a23235fa2bc36d&imgtype=jpg&er=1&src=http%3A%2F%2Fs15.sinaimg.cn%2Fmw690%2F006zervZzy77a37OySi2e%26amp%3B690',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559098159&di=84df22b901bf97803c57e8fb80cf4a34&imgtype=jpg&er=1&src=http%3A%2F%2Fi860.photobucket.com%2Falbums%2Fab166%2Fxhcmilan%2Fningenshikaku%2F17.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559098179&di=844bb7b3bbf69fa768d49b8c6b9adb60&imgtype=jpg&er=1&src=http%3A%2F%2Fwx2.sinaimg.cn%2Fwap720%2Fc25788b7ly1frwtc963m0j21120kuwo8.jpg'
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
        url: '/pages/shucehng/book4/rjshg/main'
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
