<template>
  <div>
    <i-cell-group>
      <i-cell title="阅读设置" is-link url="/pages/wode/shezhi/yuedu/main"></i-cell>
      <i-cell title="夜间模式">
        <switch slot="footer" checked />
    </i-cell>
    <i-cell title="主    题" is-link url="/pages/logs/main"></i-cell>
    <i-cell title="字    体" is-link url="/pages/logs/main"></i-cell>
    <i-cell title="插    件" is-link url="/pages/logs/main"></i-cell>
    <i-cell title="个人阅读偏好" is-link url="/pages/logs/main"></i-cell>
    <i-cell title="个人资料编辑" is-link url="/pages/logs/main"></i-cell>
    <i-cell title="账户与安全" is-link url="/pages/logs/main"></i-cell>
    <i-cell title="消息通知" is-link url="/pages/logs/main"></i-cell>
    <i-cell title="备份与同步" is-link url="/pages/logs/main"></i-cell>
    <i-cell title="清除缓存" is-link url="/pages/logs/main"></i-cell>
    <i-cell title="检查更新" is-link url="/pages/logs/main"></i-cell>
    <i-cell title="关于小程序" is-link url="/pages/logs/main"></i-cell>
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
