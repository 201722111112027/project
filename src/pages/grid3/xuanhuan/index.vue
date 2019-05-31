<template>
  <div>
    <i-notice-bar icon="systemprompt" loop>
    一大批新书即将上线
    </i-notice-bar>
   

    <i-panel title="仙侠类热门推荐">
    <i-card @click="xiuzhen" title="神魂丹圣" extra="君二代" thumb="http://img1.imgtn.bdimg.com/it/u=2386873990,1188411093&fm=26&gp=0.jpg">
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
        'https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=2053134301,1117134931&fm=26&gp=0.jpg',
        'https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=1551507617,1611419588&fm=15&gp=0.jpg',
        'https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=3162991263,309989570&fm=26&gp=0.jpg'
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
        url: '/pages/grid3/xiuzhen/main'
      })
    },
    zhuwu(){
      wx.navigateTo({
        url: '/pages/grid3/zhuwu/main'
      })
    },
    jiuyang(){
      wx.navigateTo({
        url: '/pages/grid3/jiuyang/main'
      })
    },
    xiuxian(){
      wx.navigateTo({
        url: '/pages/grid3/xiuxian/main'
      })
    },
    yishi(){
      wx.navigateTo({
        url: '/pages/grid3/yishi/main'
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
