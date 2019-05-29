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
    <text class="text"> <p>大千世界，位面交汇，万族林立，群雄荟萃，一位位来自下位面</p>的天之至尊，在这无尽世界，演绎着令人向往的传奇，追求着那主宰之路。
<p>无尽火域，炎帝执掌，万火焚苍穹。</p>
<p>武境之内，武祖之威，震慑乾坤。</p>
<p>西天之殿，百战之皇，战威无可敌。</p>
<p>北荒之丘，万墓之地，不死之主镇天地。</p>
<p>......少年自北灵境而出，骑九幽冥雀，闯向了那精彩绝伦的纷纭世界，主宰之路，谁主沉浮？</p>
<p>大千世界，万道争锋，吾为大主宰</p></text>
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
    <i-grid-item type="ghost" @click="logisiticsGZFn" i-class="no-border">
        <i-grid-icon>
            <image src="http://pic.51yuansu.com/pic2/cover/00/32/93/58110d765aa63_610.jpg" />
        </i-grid-icon>
        <i-grid-label>加入书架</i-grid-label>
    </i-grid-item>
    </i-grid> 
 <i-toast id="toast" />
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
        'http://img4.imgtn.bdimg.com/it/u=4157413056,180277472&fm=26&gp=0.jpg',
        'http://img3.imgtn.bdimg.com/it/u=435948282,1426907733&fm=26&gp=0.jpg',
        'http://img0.imgtn.bdimg.com/it/u=3821454224,340233802&fm=26&gp=0.jpg',
        'http://img3.imgtn.bdimg.com/it/u=2730843653,4052704130&fm=26&gp=0.jpg',
        'http://img2.imgtn.bdimg.com/it/u=3013196074,2059489718&fm=26&gp=0.jpg',
        'http://img4.imgtn.bdimg.com/it/u=2885733792,3261274484&fm=26&gp=0.jpg',
        'http://img3.imgtn.bdimg.com/it/u=3458523250,2512730409&fm=26&gp=0.jpg'
      ],
      indicatorDots: false,
      autoplay: true,
      interval: 5000,
      duration: 1000
    }
  },
  methods: {
    start(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
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
