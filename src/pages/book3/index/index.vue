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
    <text class="text"> 因为我既不生活在过去，也不生活在未来，我只有现在，它才是我感兴趣的。如果你能永远停留在现在，那你将是最幸福的人。你会发现沙漠里有生命，发现天空中有星星，发现士兵们打仗是因为战争是人类生活的一部分。生活就是一个节日，是一场盛大庆典。因为生活永远是，也仅仅是我们现在经历的这一刻。
——保罗·戈埃罗</text>
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
        'http://www.baidu.com/baidu.php?url=0f0000jeTx0mG_-ZTZ7jwROLqYBSm-i_B199vZ0JFm7ztqW73u1eChI4zTHv4G6WbLLsS1DYnYJYwlCVUNGj6uidCY2_ryRHJjrrVkGjM-ZIOiYIlTp9HFhZVy6ZyZQlCXo_wUiB1qG6teJugFHftK4Ac5ZfMypTifCAxJXgX_7XyFUUFkwJ6MyccVdKE1COq-JBWiN53uTndwvwzs.DR_NR2Ar5Od66kqhrPQnYPg-gYePBcnxuWooecnxuWWi1PjN0egoHPbMeqJIZ0lplPWjt5u9SAEjtJt5dzmx9L3x-EsOjvmx5v3x9lT5MY3xgdsOjksOQGsSL1sOjbsOjkls8WxfikX1BsuTEyBl7h6qYH77h24SU-CIMy9n1jv3hPh1IYePheWgguugktISOIbzIheovGYTjGo_H7IxuYSrHkzUEZk_llLHpypjDHGVQP7iOi1JHukyAp7W_ePl60.U1Yk0ZDqknZwt_MukroA4oEjdJeassKspynqnfKY5THKYxQFvTHJk8pesqp8s_n0pyYqn1mL0ATqTZP8TsKdpHY0TA-b5HDv0APGujY1P1D0Ugfqn103rNtznj640AVG5HD0TMfqnHc40ANGujY0mhbqnW0Yg1nsn-t1njn0Uynqn7ts0Z7spyfqn0Kkmv-b5H00ThIYmyTqn0KVpyfqn0KGTgfqn0K9mWYsg100ugFM5H00TZ0qn0K8IM0qna3snj0snj0sn0KVIZ0qn0KbuAqs5H00ThCqn0KhIjYs0ZKC5H00ULnqn0KBI1Ys0A4Y5H00TLCq0A71gv-bm1d8Tzd8p6KYIgnqPHczrj0kPHT1n1RzP1Dvrjn4P6Kzug7Y5HDdPH6YrHc3rjDYPWb0Tv-b5Hb4mvRzuj--PAn4PjwbPjm0mLPV5HuDPW61PRuaP1KKrRD3Pj00mynqnfKsUWYs0Z7VIjYs0Z7VT1Ys0ZGY5H00UyPxuMFEUHYsg100uA78IyF-gLK_my4GuZnqn7ts0ZK9I7qhUA7M5H00uAPGujYs0ANYpyfqQHD0mgPsmvnqn0KdTA-8mvnqn0KkUymqn0KhmLNY5H00uMGC5H00uh7Y5H00XMK_Ignqn0K9uAu_myTqnfK_uhnqn0KEIjYs0AqzTZfqnanscznsc10WnansQW0snj0snans0APzm1YknH0Lr0&word=%E7%89%A7%E7%BE%8A%E5%B0%91%E5%B9%B4%E5%A5%87%E5%B9%BB%E4%B9%8B%E6%97%85',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559097752&di=a6843f28f8c141d0d2afeaf2fef78ab5&imgtype=jpg&er=1&src=http%3A%2F%2Fimagev2.xmcdn.com%2Fgroup43%2FM05%2F17%2F7E%2FwKgKjVr5vr2Q686kAAhgMvG9vso00.jpeg%21op_type%3D5%26amp%3Bupload_type%3Dalbum%26amp%3Bdevice_type%3Dios%26amp%3Bname%3Dlarge_pop%26amp%3Bstrip%3D0%26amp%3Bquality%3D7',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558503077913&di=ccdd05911f63dc06947149184d73bbf1&imgtype=0&src=http%3A%2F%2Fimg.mp.sohu.com%2Fq_70%2Cc_zoom%2Cw_640%2Fupload%2F20170806%2Fb4deb9d7057c4b19bc8b378833d227cf_th.jpg',
        'https://ss3.bdstatic.com/70cFv8Sh_Q1YnxGkpoWK1HF6hhy/it/u=226005011,3489169462&fm=26&gp=0.jpg',
        'https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=949938761,4082951173&fm=26&gp=0.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558503077911&di=185ae87e08d787ed5b621476d7e63a3e&imgtype=0&src=http%3A%2F%2Fwww.mkaq.org%2FUploadFiles%2Fkyxy%2F2016%2F2%2F201602221501589104.jpg',
        'https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=1167003355,4231207220&fm=26&gp=0.jpg'
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
        url: '/pages/book3/muyangshaonian/main'
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
    name: "牧羊少年奇幻之旅",
    src: "https://gss1.bdstatic.com/-vo3dSag_xI4khGkpoWK1HF6hhy/baike/c0%3Dbaike116%2C5%2C5%2C116%2C38/sign=7c98a1183bd3d539d53007915bee8235/caef76094b36acaf9baf171a71d98d1000e99c8d.jpg",
    url: "/pages/book3/muyangshaonian/main",
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
