<template>
  <div>
    <!-- <div @click="toggleLeft1">
     <Button :btns="resetBtn">左边弹出3</Button>
    </div> -->
  <i-button @click="toggleLeft1" type="ghost">左边弹出1</i-button>
  <i-button @click="toggleLeft2" type="primary">左边弹出2</i-button>
  <i-button @click="toggleRight1" type="ghost">右边弹出1</i-button>
  <i-button @click="toggleRight2" type="primary">右边弹出2</i-button>
  <i-drawer mode="left" :visible="showLeft1" @close="toggleLeft1">
    <view class="demo-container">
        单击遮罩层关闭
    </view>
  </i-drawer>
  <i-drawer mode="left" :visible="showLeft2" mask-closable="false">
    <view class="demo-container">
        禁止单击遮罩关闭
        <i-button @click="toggleLeft2" type="primary">关闭</i-button>
    </view>
  </i-drawer>
  <i-drawer mode="right" :visible="showRight1" @close="toggleRight1">
    <view class="demo-container">
        单击遮罩层关闭
    </view>
  </i-drawer>
  <i-drawer mode="right" :visible="showRight2" mask-closable="false">
    <view class="demo-container">
        禁止单击遮罩关闭
        <i-button @click="toggleRight2" type="primary">关闭</i-button>
    </view>
  </i-drawer>
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
      showLeft1: false,
      showLeft2: false,
      showRight1: false,
      showRigh2: false
    }
  },
  method :{
  toggleLeft1 () {
    console.log('123')
    this.setData({
      showLeft1: this.data.showLeft1
    })
  },
  toggleLeft2 () {
    this.setData({
      showLeft2: this.data.showLeft2
    })
  },
  toggleRight1 () {
    this.setData({
      showRight1: !this.data.showRight1
    })
  },
  toggleRight2 () {
    this.setData({
      showRight2: !this.data.showRight2
    })
  },
  created () {
    let logs
    if (mpvuePlatform === 'my') {
      logs = mpvue.getStorageSync({key: 'logs'}).data || []
    } else {
      logs = mpvue.getStorageSync('logs') || []
    }
    this.logs = logs.map(log => formatTime(new Date(log)))
  }
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
