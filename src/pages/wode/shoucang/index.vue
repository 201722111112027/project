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
    <i-grid-item  @click="taizaizhi" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=2621851148,2775158789&fm=58&bpow=856&bpoh=1063" />
        </i-grid-icon>
        <i-grid-label >人间失格</i-grid-label>
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
    <i-grid-item  @click="yuqiuyu" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=3033349777,3319507516&fm=58&bpow=600&bpoh=864" />
        </i-grid-icon>
        <i-grid-label >山河之书</i-grid-label>
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
    }
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
