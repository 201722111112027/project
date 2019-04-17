<template>
  <div>
    <i-notice-bar icon="systemprompt" loop>
    一大批新书即将上线
    </i-notice-bar>
    <i-panel title="无标题输入框">
    <i-input :value="value5" placeholder="请输入收货人姓名" />
    <i-button i-class="margin" @click="click" type="primary" size="small">分类</i-button>
    </i-panel>
    <swiper 
    :indicator-dots="indicatorDots"
    :sutoplay="autoplay"
    :intervals="interval"
    :duration="duration">
    <block v-for="item in imgUrls" :key="item">
      <swiper-item>
        <image :src="item" class="slide-image" width="400" height="50" />
        </swiper-item>
        </block>
      </swiper>
    <i-grid i-class="no-border">
    <i-grid-item @click="transt" i-class="no-border">
        <i-grid-icon>
            <image src="/static/grid/1.png" />
        </i-grid-icon>
        <i-grid-label  >仙侠</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/grid/2.png" />
        </i-grid-icon>
        <i-grid-label>都市</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/grid/3.png" />
        </i-grid-icon>
        <i-grid-label>玄幻</i-grid-label>
    </i-grid-item>
    </i-grid>
    <i-grid i-class="no-border">
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/grid/4.png" />
        </i-grid-icon>
        <i-grid-label>爱情</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/grid/5.png" />
        </i-grid-icon>
        <i-grid-label>名著</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/grid/6.png" />
        </i-grid-icon>
        <i-grid-label>完本</i-grid-label>
    </i-grid-item>
</i-grid>
 <i-panel title="热门推荐">
    <!-- <view class="top-padding"> -->
    <view v-for="item in shops" :key='item' class="top-padding">
    <i-card  :title="item.name" :extra="item.type" thumb="/static/images/shop.png">
    <view slot="content">{{item.introduction}}</view>
    <view slot="footer">{{item.address}}</view>
    </i-card></view>
    <!-- </view> -->
    </i-panel>
  </div>
</template>

<script>
import card from '@/components/card'

export default {
  data () {
    return {
      imgUrls:[
        'static/images/1.jpg',
        'static/images/2.jpg',
        'static/images/3.jpg'
      ],
      indicatorDots:false,
      sutoplay:true,
      intervals:5000,
      duration1000,
      value5: '',
      shops: [],
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
    bindViewTap () {
      const url = '../logs/main'
      if (mpvuePlatform === 'wx') {
        mpvue.switchTab({ url })
      } else {
        mpvue.navigateTo({ url })
      }
    },
    clickHandle (ev) {
      console.log('clickHandle:', ev)
      // throw {message: 'custom test'}
    },
    transt(){
       console.log("123")
      wx.navigateTo({
        url: '/pages/xidian/main'
      })
    },
    click(){
      wx.navigateTo({
        url: '/pages/xidian/main'
      })
    }
  },

  created () {
    const db=wx.cloud.database({env: 'lxy599111-n9b4d'})
    db.collection('shop').get().then(
      res=>{
        this.shops=res.data
        console.log(this.shops)
      }
    )
    // wx.cloud.callFunction({name: 'user'}).then(
    //   res=>{console.log(res)}
    // )
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
p.margin
{
  background-color:yellow;
	margin-top:100px;
	margin-bottom:100px;
	margin-right:50px;
	margin-left:50px;
}
</style>
