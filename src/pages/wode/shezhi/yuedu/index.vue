<template>
  <div>
    <i-cell-group>
      <i-cell title="音量键翻页">
        <switch slot="footer" checked />
    </i-cell>
    <i-cell title="图书打开动画">
        <switch slot="footer" checked />
    </i-cell>
    <i-cell title="护眼模式" >
      <text>关闭</text>
    </i-cell>
    <i-cell title="屏幕关闭时间" >
      <text>5分钟</text>
    </i-cell>
    <i-cell title="休息提醒" >
      <text>关闭</text>
    </i-cell>
    <i-cell title="进度显示形式" >
      <text>百分比</text>
    </i-cell>
    <i-cell title="进度显示范围" >
      <text>全书</text>
    </i-cell>
     <i-cell title="全屏模式">
        <switch slot="footer" checked />
    </i-cell>
     <i-cell title="显示系统状态栏">
        <switch slot="footer" checked />
    </i-cell>
     <i-cell title="显示顶部信息区">
        <switch slot="footer" checked />
    </i-cell>
     <i-cell title="显示底部信息区">
        <switch slot="footer" checked />
    </i-cell>
     <i-cell title="按百分比显示电量">
        <switch slot="footer" checked />
    </i-cell>
     <i-cell title="书边效果">
        <switch slot="footer" checked />
    </i-cell>
     <i-cell title="横屏双翻页">
        <switch slot="footer" checked />
    </i-cell>
     <i-cell title="自动购买设置">
        <switch slot="footer" checked />
    </i-cell>
     <i-cell title="同步阅读进度和想法">
        <switch slot="footer" checked />
    </i-cell>
     <i-cell title="WiFi下字体自动下载">
        <switch slot="footer" checked />
    </i-cell>
     <i-cell title="推荐相同偏好的书到书架">
        <switch slot="footer" checked />
    </i-cell>
</i-cell-group>
  </div>
</template>

<script>
import card from '@/components/card'

export default {
  data () {
    return {
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
    }
  },

  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
.userinfo {
position: relative;
width: 750rpx;
height: 320rpx;
color: #666;
display: flex;
flex-direction: column;
align-items: center;
}
 
.userinfo-avatar {
overflow:hidden;
display: block;
width: 160rpx;
height: 160rpx;
margin: 20rpx;
margin-top: 50rpx;
border-radius: 50%;
border: 2px solid #fff;
box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.2);
}
</style>
