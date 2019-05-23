<template>
  <div><i-head color="#f759ab" >
     <i-notice-bar icon="systemprompt" loop>
    签到领福利！！！
    </i-notice-bar>
    
    <i-panel>
    <i-grid i-class="no-border">
    <i-grid-item @click="transt" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.baidu.com/6ONWsjip0QIZ8tyhnq/it/u=1952041692,3359063424&fm=58&bpow=180&bpoh=240" />
        </i-grid-icon>
        <i-grid-label >武动乾坤</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=3299594702,2547174108&fm=58&bpow=640&bpoh=878" />
        </i-grid-icon>
        <i-grid-label  >斗破苍穹</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=3642676310,272795922&fm=58&bpow=400&bpoh=504" />
        </i-grid-icon>
        <i-grid-label  >大主宰</i-grid-label>
    </i-grid-item>
     </i-grid>
    </i-panel>
    <i-panel>
     <i-grid i-class="no-border">
    <i-grid-item @click="transt" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.baidu.com/6ONWsjip0QIZ8tyhnq/it/u=2619242940,2733301503&fm=58" />
        </i-grid-icon>
        <i-grid-label >三生三世十里桃花</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=2603840089,1784701637&fm=58&bpow=417&bpoh=578" />
        </i-grid-icon>
        <i-grid-label >三生三世枕上书</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=3665834024,3736302482&fm=58&bpow=634&bpoh=800" />
        </i-grid-icon>
        <i-grid-label >三生三世步生莲</i-grid-label>
    </i-grid-item>

    <!-- <i-grid-item @click="transt" i-class="no-border">
        <i-grid-icon>
            <image src={{item.img}} />
        </i-grid-icon>
        <i-grid-label >{{item.name}}</i-grid-label>
    </i-grid-item> -->

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
  transt(){
    wx.navigateTo({
      url:'item.url'

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
