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
   <map
  id="map"
  longitude="113.324520"
  latitude="23.099994"
  scale="14"
  :controls="controls"
  bindcontroltap="controltap"
  :markers="markers"
  bindmarkertap="markertap"
  :polyline="polyline"
  @regionchange="regionchange"
  show-location
  style="width: 100%; height: 150px;"
></map>
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
      showRigh2: false,
        markers: [{
      iconPath: '/static/images/marker.png',
      id: 0,
      latitude: 23.099994,
      longitude: 113.324520,
      width: 50,
      height: 50
    }],
    polyline: [{
      points: [{
        longitude: 113.3245211,
        latitude: 23.10229
      }, {
        longitude: 113.324520,
        latitude: 23.21229
      }],
      color: '#FF0000DD',
      width: 2,
      dottedLine: true
    }],
    controls: [{
      id: 1,
      iconPath: '/static/images/location.png',
      position: {
        left: 0,
        top: 300 - 50,
        width: 50,
        height: 50
      },
      clickable: true
    }]
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
