<template>
  <div>
    <i-notice-bar icon="systemprompt" loop>
    一大批新书即将上线
    </i-notice-bar>
    <swiper
      :indicator-dots="indicatorDots"
      :autoplay="autoplay"
      :interval="interval"
      :duration="duration"
      style="height:200px"
    >
    <block v-for="item in imgUrls" :key="item">
      <swiper-item>
        <image :src="item" style="width:100%;"/>
      </swiper-item>
    </block>
  </swiper>

<i-grid i-class="no-border">
      <i-grid-item @click="goToJump(item.url)" v-for="item in grid" :key="item" i-class="no-border">
        <i-grid-icon><image :src="item.img" /></i-grid-icon>
        <i-grid-label>{{item.name}}</i-grid-label>
      </i-grid-item>
</i-grid>
    <i-panel title="图书热门推荐">
    <i-card @click="luyao" title="平凡世界" extra="路遥" thumb="http://img1.imgtn.bdimg.com/it/u=929659737,3108829528&fm=15&gp=0.jpg">
    <view slot="content">《平凡的世界》是中国作家路遥创作的一部百万字的小说。这是一部全景式地表现中国当代城乡社会生活的长篇小说，全书共三部。1986年12月首次出版。</view>
    <view slot="footer">推荐度：98%</view>
    </i-card>
    <i-card @click="qianzhongsh" title="围城" extra="钱钟书" thumb="https://gss3.bdstatic.com/7Po3dSag_xI4khGkpoWK1HF6hhy/baike/w%3D268/sign=b93945dece1b9d168ac79d67cbdfb4eb/b03533fa828ba61e672c1f2e4134970a314e59f5.jpg">
    <view slot="content">《围城》是钱钟书所著的长篇小说，是中国现代文学史上一部风格独特的讽刺小说。被誉为“新儒林外史”。第一版于1947年由上海晨光出版公司出版。故事主要写抗战初期知识分子的群相。</view>
    <view slot="footer">推荐度：95%</view>
</i-card>
<i-card @click="baoluo" title="牧羊少年奇幻之旅" extra="保罗·柯艾略" thumb="https://gss1.bdstatic.com/-vo3dSag_xI4khGkpoWK1HF6hhy/baike/c0%3Dbaike116%2C5%2C5%2C116%2C38/sign=7c98a1183bd3d539d53007915bee8235/caef76094b36acaf9baf171a71d98d1000e99c8d.jpg">
    <view slot="content">《牧羊少年奇幻之旅》是巴西作家保罗·柯艾略创作的长篇小说，首次出版于1988年。该小说运用富含哲理和诗意的语言讲述了牧羊少年圣地亚哥追寻宝藏的奇幻冒险故事，具有启发性和励志意义。</view>
    <view slot="footer">推荐度：96%</view>
</i-card>
<i-card @click="taizaizhi" title="人间失格" extra="太宰治" thumb="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=2621851148,2775158789&fm=58&bpow=856&bpoh=1063">
    <view slot="content">《人间失格》以“我”看到叶藏的三张照片后的感想开头，中间是叶藏的三篇手记，而三篇手记与照片对应，分别介绍了叶藏幼年、青年和壮年时代的经历，描述了叶藏是如何一步一步走向丧失为人资格的道路的。 [1] </view>
    <view slot="footer">推荐度：97%</view>
</i-card>
<i-card @click="yuqiuyu" title="山河之书" extra="余秋雨" thumb="https://ss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=3033349777,3319507516&fm=58&bpow=600&bpoh=864">
    <view slot="content">《山河之书》是《山居笔记》的全新修订版，余秋雨教授的很多经典文章此次都被收入其中。《山河之书》的核心篇目《我的文化山河》，从宏观上通述了中国山河的空间意义，读起来让人极为震撼。在核心篇目之后，即是余秋雨教授二十余年考察中国文化现场的脚印。</view>
    <view slot="footer">推荐度：93%</view>
</i-card>

    </i-panel>
  </div>
</template>

<script>
import card from '@/components/card'
import top from '@/data/top.json'
export default {
  data () {
    return {
      imgUrls:[
        'https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=3673068287,3206906851&fm=26&gp=0.jpg',
        'https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=2163544082,1027834145&fm=26&gp=0.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559563743859&di=befa3b264a32d3acf25303423e1a42d9&imgtype=0&src=http%3A%2F%2Fimg005.hc360.cn%2Fhb%2Fuw0c936e04784babDae03294be8465ab0c.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559563743858&di=326da2ccb798da0d19143070351a3568&imgtype=0&src=http%3A%2F%2Fimg006.hc360.cn%2Fy3%2FM01%2F0F%2FD1%2FwKhQh1WArDmEPDHJAAAAAEE39FM393.jpg',
        'https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=3822021502,4021542522&fm=26&gp=0.jpg'
      ],
      indicatorDots: false,
      autoplay: true,
      interval: 5000,
      duration: 1000,
      recommand: top,
      grid:[
      {type:"1","name":"仙侠","img":"https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=606397164,1884706880&fm=111&gp=0.jpg","url":"/pages/grid1/xianxia/main"},
      {type:"2","name":"爱情","img":"https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=899375008,44305335&fm=27&gp=0.jpg","url":"/pages/grid4/aiqing/main"},
      {type:"3","name":"名著","img":"https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=1893895325,3596953077&fm=27&gp=0.jpg","url":"/pages/grid5/mingzhu/main"},
      {type:"4","name":"完本","img":"https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=2445585430,4134671430&fm=27&gp=0.jpg","url":"/pages/grid6/wanben/main"}
      ],
    
    }
  },

  components: {
    card
  },

  methods: {
    goToJump(url){
      wx.navigateTo({url})
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
  },
}
</script>

<style scoped>
div >>> .no-border {
  border-width: 0pt;
}
.top-padding {
  padding-top: 50rpx;
}
.setting{
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-left:9px;
  margin-top: 4px;
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
