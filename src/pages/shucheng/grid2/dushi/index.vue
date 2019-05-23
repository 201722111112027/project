<template>
  <div>
    <i-notice-bar icon="systemprompt" loop>
    一大批新书即将上线
    </i-notice-bar>
   
 <!-- <i-panel title="热门推荐">
    <view class="top-padding">
    <view v-for="item in shops" :key='item' class="top-padding">
    <i-card  :title="item.name" :extra="item.type" thumb="/static/images/shop.png">
    <view slot="content">{{item.introduction}}</view>
    <view slot="footer">{{item.address}}</view>
    </i-card></view>
    </view>
    </i-panel> -->
    <i-panel title="都市类热门推荐">
    <i-card @click="xiuzhen" title="都市之仙帝归来" extra="做梦无罪" thumb="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558625575957&di=710744babaf4b7588eeb60e6f4e5eb28&imgtype=0&src=http%3A%2F%2Fhbimg.b0.upaiyun.com%2Ff7971a7744a664d20e4a37c0cdc157f2ba2acb1412fc8-Ph5paO_fw236">
    <view slot="content">修真万年，登临宇宙巅峰，而今带着万载记忆重生繁华都市。这一世我只求顺心而为，守护所爱之人，弥补前世......</view>
    <view slot="footer">推荐度：86%</view>
    </i-card>
    <i-card @click="zhuwu" title="逆天狂医" extra="火锅下小面" thumb="https://ss0.bdstatic.com/94oJfD_bAAcT8t7mm9GUKT-xh_/timg?image&quality=100&size=b4000_4000&sec=1558615449&di=586ab554197a79c05e3c28dd8700b3ce&src=http://hbimg.b0.upaiyun.com/ade774767e1e6273af7d3473ba114cbc42538def11666-1VTxs9_fw236">
    <view slot="content">逆天登仙路，一步一杀劫！萧逝水说你们逆的是天，踏的是路，我逆的是命，踏的是你们的尸骸。</view>
    <view slot="footer">推荐度：84%</view>
</i-card>
<i-card @click="jiuyang" title="重生之神级奶爸" extra="鱼未秧" thumb="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558625575950&di=fa360402e8645056ea4e9c68f58652cf&imgtype=0&src=http%3A%2F%2Fhbimg.b0.upaiyun.com%2Fef8dbf8b192a5adbafc6322b27abcd0005b785c3e474-5dBx2L_fw658">
    <view slot="content">修真界人心险恶，意外穿越，奈何重生后是一弃子，身世惨淡，幸偶遇后羿射日神功，收服九阳炉，踏平人间八方......</view>
    <view slot="footer">推荐度：73%</view>
</i-card>
<i-card @click="xiuxian" title="最强玄门弃少" extra="公子不然" thumb="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558625575945&di=0a03e99c0db86ab56b4ebe5de51fb411&imgtype=0&src=http%3A%2F%2Fwenwen.soso.com%2Fp%2F20150516%2F20150516165145-704552704.jpg">
    <view slot="content">心眼里藏着些花花肠子的街头混混，带着时灵时不灵的残破符法穿越异界，附身世家落魄少爷，且看他如何在......</view>
    <view slot="footer">推荐度：63%</view>
</i-card>
<i-card @click="yishi" title="乡村小郎中" extra="妖刀屠龙" thumb="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558625575952&di=f6d34c7bc7e88d61cb21ceb9516a3b88&imgtype=0&src=http%3A%2F%2Fhbimg.b0.upaiyun.com%2F80c4382d3e7fd3ebabbf8046870f6a12fa2c07a036823-E7Fihm_fw658">
    <view slot="content">穿越后成为已死的废柴少爷，遇上了神秘老者南叔。为亲者，为红颜，为身边最亲的人，陆少游从废柴一步步踏着...</view>
    <view slot="footer">推荐度：93%</view>
</i-card>
    </i-panel>
  </div>
</template>

<script>
import card from '@/components/card'

export default {
  data () {
    return {
      imgUrls:[
        'http://img0.imgtn.bdimg.com/it/u=1553508588,445925820&fm=15&gp=0.jpg',
        'http://img3.imgtn.bdimg.com/it/u=799192801,1646713016&fm=26&gp=0.jpg',
        'http://img5.imgtn.bdimg.com/it/u=1601665601,3863848420&fm=15&gp=0.jpg',
        'http://img5.imgtn.bdimg.com/it/u=1601665601,3863848420&fm=15&gp=0.jpg'
      ],
       indicatorDots: true,
      autoplay: true,
      interval: 5000,
      duration: 1000,
      value5: '',
      shops: [],
      isFolded: true,
      motto: 'Hello miniprograme',
      userInfo: {
        nickName: 'mpvue',
        avatarUrl: 'http://mpvue.com/assets/logo.png'
      }
    }
  },

  components: {
    card
  },

  methods: {
    xiuzhen(){
      wx.navigateTo({
        url: '/pages/pingfanshijie/main'
      })
    },
    zhuwu(){
      wx.navigateTo({
        url: '/pages/pingfanshijie/main'
      })
    },
    jiuyang(){
      wx.navigateTo({
        url: '/pages/pingfanshijie/main'
      })
    },
    xiuxian(){
      wx.navigateTo({
        url: '/pages/pingfanshijie/main'
      })
    },
    yishi(){
      wx.navigateTo({
        url: '/pages/pingfanshijie/main'
      })
    },
  },

  
}
</script>

<style scoped>
div >>> .no-border {
  border-width: 0pt;
}
.top-padding {
  padding-top: 50rpx;
}
.userinfo {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.userinfo-avatar {
  width: 128rpx;
  height: 128rpx;
  margin: 20rpx;
  border-radius: 50%;
}

.userinfo-nickname {
  color: #aaa;
}

.usermotto {
  margin-top: 150px;
}

.form-control {
  display: block;
  padding: 0 12px;
  margin-bottom: 5px;
  border: 1px solid #ccc;
}
.all{
  width:7.5rem;
  height:1rem;
  background-color:blue;
}
.all:after{
  display:block;
  content:'';
  clear:both;
}
.left{
  float:left;
  width:3rem;
  height:1rem;
  background-color:red;
}

.right{
  float:left;
  width:4.5rem;
  height:1rem;
  background-color:green;
}
.put
{
  background-color:yellow;
	margin-top:100px;
	margin-bottom:100px;
	margin-right:0px;
	margin-left:90%;
}
 
</style>
