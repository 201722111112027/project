<template>
  <div>
    <i-notice-bar icon="systemprompt" loop>
    一大批新书即将上线
    </i-notice-bar>
    <i-input i-class="put" :value="value5" placeholder="平凡世界" />
    <i-button i-class="out" @click="handleClick" type="success" shape="circle" size="small">小尺寸</i-button>
    <swiper
      :indicator-dots="indicatorDots"
      :autoplay="autoplay"
      :interval="interval"
      :duration="duration"
      style="height:250px"
    >
    <block v-for="item in imgUrls" :key="item">
      <swiper-item>
        <image :src="item" style="width:100%;"/>
      </swiper-item>
    </block>
  </swiper>
    <i-grid i-class="no-border">
    <i-grid-item @click="xianxia" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=606397164,1884706880&fm=111&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label  >仙侠</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=471158069,86109744&fm=27&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label>都市</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=3815060115,2662064952&fm=27&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label>玄幻</i-grid-label>
    </i-grid-item>
    </i-grid>
    <i-grid i-class="no-border">
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=899375008,44305335&fm=27&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label>爱情</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=1893895325,3596953077&fm=27&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label>名著</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=2445585430,4134671430&fm=27&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label>完本</i-grid-label>
    </i-grid-item>
</i-grid>
 <!-- <i-panel title="热门推荐">
    <view class="top-padding">
    <view v-for="item in shops" :key='item' class="top-padding">
    <i-card  :title="item.name" :extra="item.type" thumb="/static/images/shop.png">
    <view slot="content">{{item.introduction}}</view>
    <view slot="footer">{{item.address}}</view>
    </i-card></view>
    </view>
    </i-panel> -->
    <i-panel title="图书热门推荐">
    <i-card @click="luyao" title="平凡世界" extra="路遥" thumb="http://img1.imgtn.bdimg.com/it/u=929659737,3108829528&fm=15&gp=0.jpg">
    <view slot="content">《平凡的世界》是中国作家路遥创作的一部百万字的小说。这是一部全景式地表现中国当代城乡社会生活的长篇小说，全书共三部。1986年12月首次出版。</view>
    <view slot="footer">推荐度：98%</view>
    </i-card>
    <i-card  title="围城" extra="钱钟书" thumb="https://gss3.bdstatic.com/7Po3dSag_xI4khGkpoWK1HF6hhy/baike/w%3D268/sign=b93945dece1b9d168ac79d67cbdfb4eb/b03533fa828ba61e672c1f2e4134970a314e59f5.jpg">
    <view slot="content">《围城》是钱钟书所著的长篇小说，是中国现代文学史上一部风格独特的讽刺小说。被誉为“新儒林外史”。第一版于1947年由上海晨光出版公司出版。故事主要写抗战初期知识分子的群相。</view>
    <view slot="footer">推荐度：95%</view>
</i-card>
<i-card title="牧羊少年奇幻之旅" extra="巴西作家保罗·柯艾略" thumb="https://gss1.bdstatic.com/-vo3dSag_xI4khGkpoWK1HF6hhy/baike/c0%3Dbaike116%2C5%2C5%2C116%2C38/sign=7c98a1183bd3d539d53007915bee8235/caef76094b36acaf9baf171a71d98d1000e99c8d.jpg">
    <view slot="content">《牧羊少年奇幻之旅》是巴西作家保罗·柯艾略创作的长篇小说，首次出版于1988年。该小说运用富含哲理和诗意的语言讲述了牧羊少年圣地亚哥追寻宝藏的奇幻冒险故事，具有启发性和励志意义。</view>
    <view slot="footer">推荐度：96%</view>
</i-card>
<i-card title="人间失格" extra="太宰治" thumb="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=2621851148,2775158789&fm=58&bpow=856&bpoh=1063">
    <view slot="content">《人间失格》以“我”看到叶藏的三张照片后的感想开头，中间是叶藏的三篇手记，而三篇手记与照片对应，分别介绍了叶藏幼年、青年和壮年时代的经历，描述了叶藏是如何一步一步走向丧失为人资格的道路的。 [1] </view>
    <view slot="footer">推荐度：97%</view>
</i-card>
<i-card title="山河之书" extra="余秋雨" thumb="https://ss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=3033349777,3319507516&fm=58&bpow=600&bpoh=864">
    <view slot="content">《山河之书》是《山居笔记》的全新修订版，余秋雨教授的很多经典文章此次都被收入其中。《山河之书》的核心篇目《我的文化山河》，从宏观上通述了中国山河的空间意义，读起来让人极为震撼。在核心篇目之后，即是余秋雨教授二十余年考察中国文化现场的脚印。</view>
    <view slot="footer">推荐度：93%</view>
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
    bindViewTap () {
      const url = '../logs/main'
      if (mpvuePlatform === 'wx') {
        mpvue.switchTab({ url })
      } else {
        mpvue.navigateTo({ url })
      }
    },
    change: function (e) {
    this.setData({
      isFolded: !this.data.isFolded,
    })
    },
    clickHandle (ev) {
      console.log('clickHandle:', ev)
      // throw {message: 'custom test'}
    },
    luyao(){
      wx.navigateTo({
        url: '/pages/pingfanshijie/main'
      })
    },
    xianxia(){
      wx.navigateTo({
        url: '/pages/xianxia/main'
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
.put
{
  background-color:yellow;
	margin-top:100px;
	margin-bottom:100px;
	margin-right:0px;
	margin-left:90%;
}
 
</style>
