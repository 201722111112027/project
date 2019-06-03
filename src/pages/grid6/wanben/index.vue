<template>
  <div>
    <i-notice-bar icon="systemprompt" loop>
    一大批新书即将上线
    </i-notice-bar>
   

    <i-panel title="仙侠类热门推荐">
    <i-card @click="xiuxian" title="微微一笑很倾城" extra="顾漫" thumb="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314338246&di=cd3dead0459288fd25f1d1ad0e2eb34b&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201610%2F03%2F20161003122639_A4ZfJ.jpeg">
    <view slot="content">美女学霸贝微微，立志成为游戏工程师，化名“芦苇微微”跻身网游高手，因拒绝上传真实照片而惨遭侠侣“真水无香”无情抛弃，却意外得到江湖第一高手“一笑奈何”的垂青......</view>
    <view slot="footer">推荐度：63%</view>
</i-card>
<i-card @click="yishi" title="何以笙箫默" extra="顾漫" thumb="https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=1012176906,2583927852&fm=26&gp=0.jpg">
    <view slot="content">学时代的赵默笙，对C大法学系大才子何以琛一见倾心，开朗直率的她“死缠烂打”地倒追，与众不同的方式吸引了以琛的目光，一段纯纯的校园爱情悄悄滋生。然而......</view>
    <view slot="footer">推荐度：93%</view>
</i-card>
<i-card @click="zhuwu" title="逆天狂医" extra="火锅下小面" thumb="https://ss0.bdstatic.com/94oJfD_bAAcT8t7mm9GUKT-xh_/timg?image&quality=100&size=b4000_4000&sec=1558615449&di=586ab554197a79c05e3c28dd8700b3ce&src=http://hbimg.b0.upaiyun.com/ade774767e1e6273af7d3473ba114cbc42538def11666-1VTxs9_fw236">
    <view slot="content">逆天登仙路，一步一杀劫！萧逝水说你们逆的是天，踏的是路，我逆的是命，踏的是你们的尸骸。</view>
    <view slot="footer">推荐度：84%</view>
</i-card>
<i-card @click="jiuyang" title="重生之神级奶爸" extra="鱼未秧" thumb="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558625575950&di=fa360402e8645056ea4e9c68f58652cf&imgtype=0&src=http%3A%2F%2Fhbimg.b0.upaiyun.com%2Fef8dbf8b192a5adbafc6322b27abcd0005b785c3e474-5dBx2L_fw658">
    <view slot="content">修真界人心险恶，意外穿越，奈何重生后是一弃子，身世惨淡，幸偶遇后羿射日神功，收服九阳炉，踏平人间八方......</view>
    <view slot="footer">推荐度：73%</view>
</i-card>
<i-card @click="luyao" title="平凡世界" extra="路遥" thumb="http://img1.imgtn.bdimg.com/it/u=929659737,3108829528&fm=15&gp=0.jpg">
    <view slot="content">《平凡的世界》是中国作家路遥创作的一部百万字的小说。这是一部全景式地表现中国当代城乡社会生活的长篇小说，全书共三部。1986年12月首次出版。</view>
    <view slot="footer">推荐度：98%</view>
    </i-card>
    <i-card @click="qianzhongsh" title="围城" extra="钱钟书" thumb="https://gss3.bdstatic.com/7Po3dSag_xI4khGkpoWK1HF6hhy/baike/w%3D268/sign=b93945dece1b9d168ac79d67cbdfb4eb/b03533fa828ba61e672c1f2e4134970a314e59f5.jpg">
    <view slot="content">《围城》是钱钟书所著的长篇小说，是中国现代文学史上一部风格独特的讽刺小说。被誉为“新儒林外史”。第一版于1947年由上海晨光出版公司出版。故事主要写抗战初期知识分子的群相。</view>
    <view slot="footer">推荐度：95%</view>
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
    luyao(){
      wx.navigateTo({
        url: '/pages/book1/index/main'
      })
    },
    qianzhongsh(){
      wx.navigateTo({
        url: '/pages/book2/index/main'
      })
    },
    zhuwu(){
      wx.navigateTo({
        url: '/pages/grid2/zhuwu/main'
      })
    },
    jiuyang(){
      wx.navigateTo({
        url: '/pages/grid2/jiuyang/main'
      })
    },
   xiuxian(){
      wx.navigateTo({
        url: '/pages/grid4/xiuxian/main'
      })
    },
    yishi(){
      wx.navigateTo({
        url: '/pages/grid4/yishi/main'
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
