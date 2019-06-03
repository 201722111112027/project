<template>
  <div>
    <i-notice-bar icon="systemprompt" loop>
    今日免费！！！
    </i-notice-bar>
    <i-card @click="xiuzhen" title="修真万年归来" extra="缸里有米" thumb="http://img1.imgtn.bdimg.com/it/u=929659737,3108829528&fm=15&gp=0.jpg">
    <view slot="content">修真万年，登临宇宙巅峰，而今带着万载记忆重生繁华都市。这一世我只求顺心而为，守护所爱之人，弥补前世......</view>
    <view slot="footer">推荐度：86%</view>
    </i-card>
    <i-card @click="zhuwu" title="诛天武帝" extra="云七公子" thumb="https://gss3.bdstatic.com/7Po3dSag_xI4khGkpoWK1HF6hhy/baike/w%3D268/sign=b93945dece1b9d168ac79d67cbdfb4eb/b03533fa828ba61e672c1f2e4134970a314e59f5.jpg">
    <view slot="content">逆天登仙路，一步一杀劫！萧逝水说你们逆的是天，踏的是路，我逆的是命，踏的是你们的尸骸。</view>
    <view slot="footer">推荐度：84%</view>
</i-card>
<i-card @click="jiuyang" title="九阳至尊" extra="剪刀石头布" thumb="https://gss1.bdstatic.com/-vo3dSag_xI4khGkpoWK1HF6hhy/baike/c0%3Dbaike116%2C5%2C5%2C116%2C38/sign=7c98a1183bd3d539d53007915bee8235/caef76094b36acaf9baf171a71d98d1000e99c8d.jpg">
    <view slot="content">修真界人心险恶，意外穿越，奈何重生后是一弃子，身世惨淡，幸偶遇后羿射日神功，收服九阳炉，踏平人间八方......</view>
    <view slot="footer">推荐度：73%</view>
</i-card>
<i-card @click="xiuxian" title="修仙狂徒" extra="王小蛮" thumb="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=2621851148,2775158789&fm=58&bpow=856&bpoh=1063">
    <view slot="content">心眼里藏着些花花肠子的街头混混，带着时灵时不灵的残破符法穿越异界，附身世家落魄少爷，且看他如何在......</view>
    <view slot="footer">推荐度：63%</view>
</i-card>
<i-card @click="yishi" title="异世灵武天下" extra="禹枫" thumb="https://ss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=3033349777,3319507516&fm=58&bpow=600&bpoh=864">
    <view slot="content">穿越后成为已死的废柴少爷，遇上了神秘老者南叔。为亲者，为红颜，为身边最亲的人，陆少游从废柴一步步踏着...</view>
    <view slot="footer">推荐度：93%</view>
</i-card>
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
  </div>
</template>

<script>
import card from '@/components/card'

export default {
  data () {
    return {
      imgUrls:[
        '//timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1555729898350&di=92a67fa7c6433b9f60079a62e457af64&imgtype=0&src=http%3A%2F%2Fv1.qzone.cc%2Fpic%2F201608%2F15%2F20%2F19%2F57b1b343297d4387.jpeg%2521600x600.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1555729898350&di=0f2e2beb6657de0268d6473eabc0dafc&imgtype=0&src=http%3A%2F%2Fs9.rr.itc.cn%2Fr%2FwapChange%2F20173_31_17%2Fa0zvhl1070816226619.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1555729898346&di=53120318aab25723f14e4c70be9463b8&imgtype=0&src=http%3A%2F%2Fimg.mp.sohu.com%2Fupload%2F20170513%2F8e0db367b0a44076adbdf96271cd8b4b_th.png'
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
        url: '/pages/book1/index/main'
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
