<template>
  <div><i-head color="#f759ab" >
     <i-notice-bar icon="systemprompt" loop>
    签到领福利！！！
    </i-notice-bar>
    
    <i-panel>
    <i-grid i-class="no-border">
    <i-grid-item @click="transt1" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.baidu.com/6ONWsjip0QIZ8tyhnq/it/u=1952041692,3359063424&fm=58&bpow=180&bpoh=240" />
        </i-grid-icon>
        <i-grid-label >武动乾坤</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt2" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=3299594702,2547174108&fm=58&bpow=640&bpoh=878" />
        </i-grid-icon>
        <i-grid-label  >斗破苍穹</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt3" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=3642676310,272795922&fm=58&bpow=400&bpoh=504" />
        </i-grid-icon>
        <i-grid-label  >大主宰</i-grid-label>
    </i-grid-item>
     </i-grid>
    </i-panel>
    <i-panel>
     <i-grid i-class="no-border">
    <i-grid-item @click="transt4" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.baidu.com/6ONWsjip0QIZ8tyhnq/it/u=2619242940,2733301503&fm=58" />
        </i-grid-icon>
        <i-grid-label >三生三世十里桃花</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt5" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=2603840089,1784701637&fm=58&bpow=417&bpoh=578" />
        </i-grid-icon>
        <i-grid-label >三生三世枕上书</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt6" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=3665834024,3736302482&fm=58&bpow=634&bpoh=800" />
        </i-grid-icon>
        <i-grid-label >三生三世步生莲</i-grid-label>
    </i-grid-item>
    </i-grid>
    </i-panel>

     <i-panel>
     <i-grid i-class="no-border">
    <i-grid-item  @click="luyao" i-class="no-border">
        <i-grid-icon>
            <image src="http://img1.imgtn.bdimg.com/it/u=929659737,3108829528&fm=15&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label >平凡世界</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="qianzhongsh" i-class="no-border">
        <i-grid-icon>
            <image src="https://gss3.bdstatic.com/7Po3dSag_xI4khGkpoWK1HF6hhy/baike/w%3D268/sign=b93945dece1b9d168ac79d67cbdfb4eb/b03533fa828ba61e672c1f2e4134970a314e59f5.jpg" />
        </i-grid-icon>
        <i-grid-label >围城</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="baoluo" i-class="no-border">
        <i-grid-icon>
            <image src="https://gss1.bdstatic.com/-vo3dSag_xI4khGkpoWK1HF6hhy/baike/c0%3Dbaike116%2C5%2C5%2C116%2C38/sign=7c98a1183bd3d539d53007915bee8235/caef76094b36acaf9baf171a71d98d1000e99c8d.jpg" />
        </i-grid-icon>
        <i-grid-label >牧羊少年奇幻之旅</i-grid-label>
    </i-grid-item>
    </i-grid>
    </i-panel>

    <i-panel>
     <i-grid i-class="no-border">
    <i-grid-item  @click="taizaizhi" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=2621851148,2775158789&fm=58&bpow=856&bpoh=1063" />
        </i-grid-icon>
        <i-grid-label >人间失格</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="yuqiuyu" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=3033349777,3319507516&fm=58&bpow=600&bpoh=864" />
        </i-grid-icon>
        <i-grid-label >山河之书</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="xiuzhen" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=1978681538,2729255002&fm=26&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label >修真万年归来</i-grid-label>
    </i-grid-item>
    </i-grid>
    </i-panel>

  <i-panel>
     <i-grid i-class="no-border">
    <i-grid-item  @click="zhuwu" i-class="no-border">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559316455881&di=1f6629a9a8cb51abea8bc137561ba38e&imgtype=0&src=http%3A%2F%2F5b0988e595225.cdn.sohucs.com%2Fimages%2F20180626%2Fa3feb9b12b7f42d98dad6f2bee80eeee.jpeg" />
        </i-grid-icon>
        <i-grid-label >诛天武帝</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="jiuyang" i-class="no-border">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559316455881&di=22859135668e1f2854a57b4f69c85cc4&imgtype=0&src=http%3A%2F%2Fn.sinaimg.cn%2Ffront%2F24%2Fw494h330%2F20181219%2FWh-F-hqnkypq9787687.jpg" />
        </i-grid-icon>
        <i-grid-label >九阳至尊</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="xiuxian" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=2386873990,1188411093&fm=26&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label >修仙狂徒</i-grid-label>
    </i-grid-item>
    </i-grid>
    </i-panel>

<i-panel>
     <i-grid i-class="no-border">
    <i-grid-item  @click="yishi" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=3367722916,4062242920&fm=26&gp=0.jpg"/>
        </i-grid-icon>
        <i-grid-label >异世灵武天下</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="zhuwu2" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.bdstatic.com/94oJfD_bAAcT8t7mm9GUKT-xh_/timg?image&quality=100&size=b4000_4000&sec=1558615449&di=586ab554197a79c05e3c28dd8700b3ce&src=http://hbimg.b0.upaiyun.com/ade774767e1e6273af7d3473ba114cbc42538def11666-1VTxs9_fw236" />
        </i-grid-icon>
        <i-grid-label > 逆天狂医</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="xiuzhen2" i-class="no-border">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558625575957&di=710744babaf4b7588eeb60e6f4e5eb28&imgtype=0&src=http%3A%2F%2Fhbimg.b0.upaiyun.com%2Ff7971a7744a664d20e4a37c0cdc157f2ba2acb1412fc8-Ph5paO_fw236" />
        </i-grid-icon>
        <i-grid-label >都市之仙帝归来</i-grid-label>
    </i-grid-item>
    </i-grid>
    </i-panel>
    <i-panel>
     <i-grid i-class="no-border">
    <i-grid-item  @click="jiuyang2" i-class="no-border">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558625575950&di=fa360402e8645056ea4e9c68f58652cf&imgtype=0&src=http%3A%2F%2Fhbimg.b0.upaiyun.com%2Fef8dbf8b192a5adbafc6322b27abcd0005b785c3e474-5dBx2L_fw658"/>
         </i-grid-icon>
        <i-grid-label >重生之神级奶爸</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="xiuxian2" i-class="no-border">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558625575945&di=0a03e99c0db86ab56b4ebe5de51fb411&imgtype=0&src=http%3A%2F%2Fwenwen.soso.com%2Fp%2F20150516%2F20150516165145-704552704.jpg" />
        </i-grid-icon>
        <i-grid-label >最强玄门弃少</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="yishi2" i-class="no-border">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1558625575952&di=f6d34c7bc7e88d61cb21ceb9516a3b88&imgtype=0&src=http%3A%2F%2Fhbimg.b0.upaiyun.com%2F80c4382d3e7fd3ebabbf8046870f6a12fa2c07a036823-E7Fihm_fw658" />
        </i-grid-icon>
        <i-grid-label >乡村小郎中</i-grid-label>
    </i-grid-item>
    </i-grid>
    </i-panel>    

</i-head>
      
  </div>
</template>

<script>
import card from '@/components/card'

export default {
  data () {
    return {
      current_scroll: 'tab1',
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
   onLoad: function(options) {
      var dataTemp = decodeURIComponent(options.dataList);//函数可把字符串作为 URI 组件进行解码。
      var Traces = JSON.parse(dataTemp);//航一页传过来的json字符串转化成json数组  物流信息进度
      this.setData({
        Traces: Traces
      })
  },
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
    baoluo(){
      wx.navigateTo({
        url: '/pages/book3/index/main'
      })
    },
    taizaizhi(){
      wx.navigateTo({
        url: '/pages/book4/index/main'
      })
    },
    yuqiuyu(){
      wx.navigateTo({
        url: '/pages/book5/index/main'
      })
    },
    transt1(){
      wx.navigateTo({
        url: '/pages/shujia/wudong/main'
      })
    },
    transt2(){
      wx.navigateTo({
        url: '/pages/shujia/doupo/main'
      })
    },
    transt3(){
      wx.navigateTo({
        url: '/pages/shujia/dazhuzai/main'
      })
    },
    transt4(){
      wx.navigateTo({
        url: '/pages/shujia/shilitaohua/main'
      })
    },
    transt6(){
      wx.navigateTo({
        url: '/pages/shujia/zhenshangshu/main'
      })
    },
    transt6(){
      wx.navigateTo({
        url: '/pages/shujia/bushenglian/main'
      })
    },
    xiuzhen(){
      wx.navigateTo({
        url: '/pages/grid1/xiuzhen/main'
      })
    },
    zhuwu(){
      wx.navigateTo({
        url: '/pages/grid1/zhuwu/main'
      })
    },
    jiuyang(){
      wx.navigateTo({
        url: '/pages/grid1/jiuyang/main'
      })
    },
    xiuxian(){
      wx.navigateTo({
        url: '/pages/grid1/xiuxian/main'
      })
    },
    yishi(){
      wx.navigateTo({
        url: '/pages/grid1/yishi/main'
      })
    },
    xiuzhen2(){
      wx.navigateTo({
        url: '/pages/grid2/xiuzhen/main'
      })
    },
    zhuwu2(){
      wx.navigateTo({
        url: '/pages/grid2/zhuwu/main'
      })
    },
    jiuyang2(){
      wx.navigateTo({
        url: '/pages/grid2/jiuyang/main'
      })
    },
    xiuxian2(){
      wx.navigateTo({
        url: '/pages/grid2/xiuxian/main'
      })
    },
    yishi2(){
      wx.navigateTo({
        url: '/pages/grid2/yishi/main'
      })
    },
  },

  created () {
    // let app = getApp()
  }
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
</style>
