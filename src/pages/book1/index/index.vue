<template>
  <div class="counter-warp" >
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
        </view>
    </i-panel>
    <i-panel class="panel">
    <text class="text"> 青年，青年！无论受怎样的挫折和打击，都要咬着牙冠挺住，因为你们完全有机会重建生活；只要不灰心丧气，每一次挫折，只不过是通往新境界的一块普通绊脚石而绝不会置人于死命。                        ——路遥</text>
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
    <!-- <i-grid v-for="item in recommand" :key="item" i-class="no-border">
      <i-grid-item @click="start(option)" class="test">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1557854121615&di=b6b001204cc993e8bd6684863bf2dd86&imgtype=0&src=http%3A%2F%2Fpic.51yuansu.com%2Fpic2%2Fcover%2F00%2F32%2F00%2F5810d7724ac54_610.jpg" />
        </i-grid-icon>
        <i-grid-label>免费试读</i-grid-label>
    </i-grid-item>
    </i-grid>  -->
      <!-- <view class="setting">
        <button class="button" @click='jump'>购票</button>
        <button class="button" @click='jump'>购票</button>
        <button class="button" @click='jump'>购票</button>
      </view> -->
  </div>
</template>

<script>
// Use Vuex
import store from './store'
import top from '@/data/top.json'

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
      duration: 1000,
      recommand: top
    }
  },
  methods: {
    start(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
      })
     
    },
    down(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
      })
    },
    
    logisiticsGZFn(){
      wx.showToast({
      title: '成功添加',
      icon: 'success',
      duration: 2000
      })
      const db = wx.cloud.database({ env: 'lxy599111-n9b4d' })
    db.collection('shujia').add({
    // data 字段表示需新增的 JSON 数据
    data: {
    // _id: 'todo-identifiant-aleatoire', // 可选自定义 _id，在此处场景下用数据库自动分配的就可以了
    name: "平凡世界",
    src: "http://img1.imgtn.bdimg.com/it/u=929659737,3108829528&fm=15&gp=0.jpg",
    url: "/pages/book1/pfsj/main",
    tags: [
      "cloud",
      "database"
    ],
    // // 为待办事项添加一个地理位置（113°E，23°N）
    // location: new db.Geo.Point(113, 23),
    done: false
  },
  success: function(res) {
    // res 是一个对象，其中有 _id 字段标记刚创建的记录的 id
    console.log(res)
  }
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
