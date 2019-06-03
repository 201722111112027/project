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
    <text class="text"> 唐末一个逃难者在严寒之夜被扯进了一扇柴门，宋代一个书生落水被路人救起，这可能就算我们的祖先，一场灭绝性的征剿不知被谁劝阻，一所最小的私塾在某个荒村开张。这些事情，也可能远远的与我有关，因此我们区区五尺之躯，不知道沉淀了多少善良，文化是一种感恩，我们要懂得把他们完全唤醒”
——余秋雨</text>
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
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559098343&di=08a4297f0909f25201215a11a0a580fa&imgtype=jpg&er=1&src=http%3A%2F%2Fbook.img.ireader.com%2Fgroup6%2FM00%2F64%2F58%2FCmQUNlZxKWyET7bnAAAAAEuAA8k030172610.jpg%3Fv%3D8v0VrD2-',
        'https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=2076386763,3164677909&fm=11&gp=0.jpg',
        'https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=1531787081,3113287356&fm=26&gp=0.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559098378&di=0cd6622427fb30bbec1b7774308739f8&imgtype=jpg&er=1&src=http%3A%2F%2F5b0988e595225.cdn.sohucs.com%2Fimages%2F20171204%2F41815c46e7b346ae8ed3e8956975aacc.jpeg',
        'https://ss3.bdstatic.com/70cFv8Sh_Q1YnxGkpoWK1HF6hhy/it/u=2070827847,4188947884&fm=26&gp=0.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558503748016&di=290d9d44e74686d89fbfacdab40b14a5&imgtype=0&src=http%3A%2F%2Fi.ce.cn%2Fintl%2Fzhuanti%2Fydylx%2Fcscq_286187%2Ftp%2F201604%2F11%2FW020160413721089383801.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558503748013&di=49debdcef4daef5f6e7e82e09e5b2097&imgtype=0&src=http%3A%2F%2Fp2.pccoo.cn%2Fbbs%2F20141106%2F2014110616261353746620.jpg'
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
        url: '/pages/book5/shanhezhishu/main'
      })
    },
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
