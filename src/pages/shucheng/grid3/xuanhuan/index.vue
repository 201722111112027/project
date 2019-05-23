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
    <i-panel title="仙侠类热门推荐">
    <i-card @click="xiuzhen" title="神魂丹圣" extra="君二代" thumb="data:image/jpeg;base64,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">
    <view slot="content">修真万年，登临宇宙巅峰，而今带着万载记忆重生繁华都市。这一世我只求顺心而为，守护所爱之人，弥补前世......</view>
    <view slot="footer">推荐度：86%</view>
    </i-card>
    <i-card @click="zhuwu" title="魔帝归来" extra="鸡汤豆脑" thumb="https://gss3.bdstatic.com/7Po3dSag_xI4khGkpoWK1HF6hhy/baike/w%3D268/sign=b93945dece1b9d168ac79d67cbdfb4eb/b03533fa828ba61e672c1f2e4134970a314e59f5.jpg">
    <view slot="content">逆天登仙路，一步一杀劫！萧逝水说你们逆的是天，踏的是路，我逆的是命，踏的是你们的尸骸。</view>
    <view slot="footer">推荐度：84%</view>
</i-card>
<i-card @click="jiuyang" title="武道圣帝" extra="鱼大鲲" thumb="https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=2683510064,1206962688&fm=26&gp=0.jpg">
    <view slot="content">修真界人心险恶，意外穿越，奈何重生后是一弃子，身世惨淡，幸偶遇后羿射日神功，收服九阳炉，踏平人间八方......</view>
    <view slot="footer">推荐度：73%</view>
</i-card>
<i-card @click="xiuxian" title="无敌战神" extra="青玄" thumb="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=2621851148,2775158789&fm=58&bpow=856&bpoh=1063">
    <view slot="content">心眼里藏着些花花肠子的街头混混，带着时灵时不灵的残破符法穿越异界，附身世家落魄少爷，且看他如何在......</view>
    <view slot="footer">推荐度：63%</view>
</i-card>
<i-card @click="yishi" title="绝世斗神" extra="灼炎" thumb="https://ss3.bdstatic.com/70cFv8Sh_Q1YnxGkpoWK1HF6hhy/it/u=2202823712,1515862429&fm=15&gp=0.jpg">
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
        'https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=1301019939,2414145904&fm=26&gp=0.jpg',
        'https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=1280191097,1878141398&fm=26&gp=0.jpg',
        'https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=2053134301,1117134931&fm=26&gp=0.jpg'
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
