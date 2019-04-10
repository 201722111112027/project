<template>
  <div>
    <i-panel title="吃货推荐">
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
import { formatTime } from '@/utils/index'
import card from '@/components/card'

export default {
  components: {
    card
  },

  data () {
    return {
      shop: [],
      motto: 'Hello miniprograme',
      userInfo: {
        nickName: 'mpvue',
        avatarUrl: 'http://mpvue.com/assets/logo.png'
      },
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

<style>
.log-list {
  display: flex;
  flex-direction: column;
  padding: 40rpx;
}

.log-item {
  margin: 10rpx;
}
</style>
