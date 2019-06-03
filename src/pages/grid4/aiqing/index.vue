<template>
  <div>
    <i-notice-bar icon="systemprompt" loop>
    一大批新书即将上线
    </i-notice-bar>
   
 <!-- <i-panel title="热门推荐">
    <view class="top-padding">
    <view v-for="item in shops" :key='item' class="top-padding">
    <i-card  :title="item.name" :extra="item.type" thumb="/static/images/shop.png">
    <view slot="content">{{item.introduction}}</view>
    <view slot="footer">{{item.address}}</view>
    </i-card></view>
    </view>
    </i-panel> -->
    <i-panel title="仙侠类热门推荐">
    <i-card @click="xiuzhen" title="致我们暖暖的小时光" extra="赵乾" thumb="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559908504&di=321348aaec92b6cebd7ff908816ea82f&imgtype=jpg&er=1&src=http%3A%2F%2Fimage.ijq.tv%2F201808%2F10%2F15-34-52-40-10.jpg">
    <view slot="content">司徒末（邢菲 饰）毕业在即，从小便习惯服从安排的她对前途迷茫懵懂，随波逐流地尝试各种安排，总是鼓不起勇气为自己做出选择。因新老校区并校，物理系的高材生顾未易（林一 饰）闯入司徒末的生活......</view>
    <view slot="footer">推荐度：86%</view>
    </i-card>
    <i-card @click="zhuwu" title="致我们单纯的小美好" extra="赵乾" thumb="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559908334&di=cd29c38d475b1968ea892e550703a4bc&imgtype=jpg&er=1&src=http%3A%2F%2Fy.gtimg.cn%2Fmusic%2Fphoto_new%2FT015R640x360M101001oJUbF4fVuh4.jpg">
    <view slot="content">蠢萌活泼的元气少女陈小希（沈月饰）从学生时代起一直追逐着邻家男孩江辰（胡一天饰）的脚步，面对陈小希的强烈倒追，傲娇高冷的学霸江辰不为所动。大学毕业后......</view>
    <view slot="footer">推荐度：84%</view>
</i-card>
<i-card @click="jiuyang" title="我只喜欢你" extra="赵乔一" thumb="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559313913979&di=d7145249aa2263c7cac8f37ed51ec923&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201509%2F04%2F20150904204200_rPwNS.jpeg">
    <view slot="content">讲述了一个女孩挫折不断的成长，和一个男孩温柔守护的故事。一场懵懂恋爱，成为生命中的一束光，相互照亮彼此，从校服到婚纱，爱让他们成为更好的人。</view>
    <view slot="footer">推荐度：73%</view>
</i-card>
<i-card @click="xiuxian" title="微微一笑很倾城" extra="顾漫" thumb="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559314338246&di=cd3dead0459288fd25f1d1ad0e2eb34b&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201610%2F03%2F20161003122639_A4ZfJ.jpeg">
    <view slot="content">美女学霸贝微微，立志成为游戏工程师，化名“芦苇微微”跻身网游高手，因拒绝上传真实照片而惨遭侠侣“真水无香”无情抛弃，却意外得到江湖第一高手“一笑奈何”的垂青......</view>
    <view slot="footer">推荐度：63%</view>
</i-card>
<i-card @click="yishi" title="何以笙箫默" extra="顾漫" thumb="https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=1012176906,2583927852&fm=26&gp=0.jpg">
    <view slot="content">学时代的赵默笙，对C大法学系大才子何以琛一见倾心，开朗直率的她“死缠烂打”地倒追，与众不同的方式吸引了以琛的目光，一段纯纯的校园爱情悄悄滋生。然而......</view>
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
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559909872&di=a578a0f7afb06a23370714547bacad5b&imgtype=jpg&er=1&src=http%3A%2F%2Fimage.biaobaiju.com%2Fuploads%2F20181220%2F23%2F1545320881-jxIvBiFsVS.jpg',
        'https://ss3.bdstatic.com/70cFv8Sh_Q1YnxGkpoWK1HF6hhy/it/u=3373546447,1707066306&fm=26&gp=0.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559315196479&di=6903bd96043d70b037615833765c958d&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201704%2F07%2F20170407002432_e2KYm.thumb.700_0.jpeg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559315196478&di=e8171aae040b0164d9ee34258d7d8c55&imgtype=0&src=http%3A%2F%2Fimage.biaobaiju.com%2Fuploads%2F20181220%2F23%2F1545320882-BfMgrThVZO.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559315196478&di=b0d46d6c545a10a57c41d918b21ecd01&imgtype=0&src=http%3A%2F%2Fimage.biaobaiju.com%2Fuploads%2F20181220%2F23%2F1545320881-mjxwaVNfWh.jpg'
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
    xiuzhen(){
      wx.navigateTo({
        url: '/pages/grid4/xiuzhen/main'
      })
    },
    zhuwu(){
      wx.navigateTo({
        url: '/pages/grid4/zhuwu/main'
      })
    },
    jiuyang(){
      wx.navigateTo({
        url: '/pages/grid4/jiuyang/main'
      })
    },
    xiuxian(){
      wx.navigateTo({
        url: '/pages/grid4/xiuxian/main'
      })
    },
    yishi(){
      wx.navigateTo({
        url: '/pages/grid4/yishi/main'
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
