<template>
  <div><i-head color="#f759ab" >
     <i-notice-bar icon="systemprompt" loop>
    签到领福利！！！
    </i-notice-bar>
    
    <!-- <i-grid i-class="no-border">
    <i-grid-item @click="transt1" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.baidu.com/6ONWsjip0QIZ8tyhnq/it/u=1952041692,3359063424&fm=58&bpow=180&bpoh=240" />
        </i-grid-icon>
        <i-grid-label >武动乾坤</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt2" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=3299594702,2547174108&fm=58&bpow=640&bpoh=878" />
        </i-grid-icon>
        <i-grid-label  >斗破苍穹</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt3" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=3642676310,272795922&fm=58&bpow=400&bpoh=504" />
        </i-grid-icon>
        <i-grid-label  >大主宰</i-grid-label>
    </i-grid-item>
     </i-grid>
    </i-panel>
    <i-panel>
     <i-grid i-class="no-border">
    <i-grid-item @click="transt4" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.baidu.com/6ONWsjip0QIZ8tyhnq/it/u=2619242940,2733301503&fm=58" />
        </i-grid-icon>
        <i-grid-label >三生三世十里桃花</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt5" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=2603840089,1784701637&fm=58&bpow=417&bpoh=578" />
        </i-grid-icon>
        <i-grid-label >三生三世枕上书</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="transt6" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=3665834024,3736302482&fm=58&bpow=634&bpoh=800" />
        </i-grid-icon>
        <i-grid-label >三生三世步生莲</i-grid-label>
    </i-grid-item>
    </i-grid>
    </i-panel>

     <i-panel>
     <i-grid i-class="no-border">
    <i-grid-item  @click="luyao" i-class="no-border">
        <i-grid-icon>
            <image src="http://img1.imgtn.bdimg.com/it/u=929659737,3108829528&fm=15&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label >平凡世界</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="qianzhongsh" i-class="no-border">
        <i-grid-icon>
            <image src="https://gss3.bdstatic.com/7Po3dSag_xI4khGkpoWK1HF6hhy/baike/w%3D268/sign=b93945dece1b9d168ac79d67cbdfb4eb/b03533fa828ba61e672c1f2e4134970a314e59f5.jpg" />
        </i-grid-icon>
        <i-grid-label >围城</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="baoluo" i-class="no-border">
        <i-grid-icon>
            <image src="https://gss1.bdstatic.com/-vo3dSag_xI4khGkpoWK1HF6hhy/baike/c0%3Dbaike116%2C5%2C5%2C116%2C38/sign=7c98a1183bd3d539d53007915bee8235/caef76094b36acaf9baf171a71d98d1000e99c8d.jpg" />
        </i-grid-icon>
        <i-grid-label >牧羊少年奇幻之旅</i-grid-label>
    </i-grid-item>
    </i-grid>
    </i-panel>

    <i-panel>
     <i-grid i-class="no-border">
    <i-grid-item  @click="taizaizhi" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=2621851148,2775158789&fm=58&bpow=856&bpoh=1063" />
        </i-grid-icon>
        <i-grid-label >人间失格</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="yuqiuyu" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=3033349777,3319507516&fm=58&bpow=600&bpoh=864" />
        </i-grid-icon>
        <i-grid-label >山河之书</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="xiuzhen" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=1978681538,2729255002&fm=26&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label >修真万年归来</i-grid-label>
    </i-grid-item>
    </i-grid>
    </i-panel>

  <i-panel>
     <i-grid i-class="no-border">
    <i-grid-item  @click="zhuwu" i-class="no-border">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559316455881&di=1f6629a9a8cb51abea8bc137561ba38e&imgtype=0&src=http%3A%2F%2F5b0988e595225.cdn.sohucs.com%2Fimages%2F20180626%2Fa3feb9b12b7f42d98dad6f2bee80eeee.jpeg" />
        </i-grid-icon>
        <i-grid-label >诛天武帝</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="jiuyang" i-class="no-border">
        <i-grid-icon>
            <image src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1559316455881&di=22859135668e1f2854a57b4f69c85cc4&imgtype=0&src=http%3A%2F%2Fn.sinaimg.cn%2Ffront%2F24%2Fw494h330%2F20181219%2FWh-F-hqnkypq9787687.jpg" />
        </i-grid-icon>
        <i-grid-label >九阳至尊</i-grid-label>
    </i-grid-item>
    <i-grid-item  @click="xiuxian" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=2386873990,1188411093&fm=26&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label >修仙狂徒</i-grid-label>
    </i-grid-item>
    </i-grid> -->

    


    <!--

    <view class='header-container'>
        <image class='bg' :src='option.img'/>
        <view class='setting'>
          <image :src='option.img' style="width:250rpx;height:360rpx;"/>
          <text style="padding:8px;line-height:30px">
            <text class="movie">{{option.name}}</text>
          </text>
        </view>
    </view> -->
 

</i-head>
    <i-grid i-class="no-border">
      <i-grid-item v-for="item in books" :key="item" @click="goToJump(item.url)" class="grid">
        <i-grid-icon><image :src="item.src" /></i-grid-icon>
        <i-grid-label>{{item.name}}</i-grid-label>
      </i-grid-item>
    </i-grid>


  </div>
</template>

<script>
import card from '@/components/card'

export default {
  
  data () {
    return{ 
      books:[]
    }
  },
  
  components: {
    card
  },

  // methods: {
  
 

  //   goToJump(url){
  //     wx.navigateTo({
  //       url
  //     })
  //   },
  // },

  //  created () {
  //   const db = wx.cloud.database({ env: 'lxy599111-n9b4d' })
  //   db.collection('shujia').get().then(
  //     res => {
  //       console.log(res.data)
  //       this.books = res.data
  //     }
  //   )
  // }

}
</script>

<style scoped>
div >>> .no-border {
 border-width: 0pt;
}

.grids {
    position: relative;
    overflow: hidden;
}
 
 .grids:before {
    content: " ";
    position: absolute;
    left: 0;
    top: 0;
    right: 0;
    height: 1px;
    border-top: 1px solid #d9d9d9;
    color: #d9d9d9;
    -webkit-transform-origin: 0 0;
    transform-origin: 0 0;
    -webkit-transform: scaleY(0.5);
    transform: scaleY(0.5);
} 
 
 .grids:after {
    content: " ";
    position: absolute;
    left: 0;
    top: 0;
    width: 1px;
    bottom: 0;
    border-left: 1px solid #d9d9d9;
    color: #d9d9d9;
    -webkit-transform-origin: 0 0;
    transform-origin: 0 0;
    -webkit-transform: scaleX(0.5);
    transform: scaleX(0.5);
} 
 
 /* 睁大眼睛看这里，尤其下面的width，50%是两列，33.3333%是三列，25%是四列 */
 
.grid {
    position: relative;
    float: left;
    
    width: 50%;                                    
    
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
