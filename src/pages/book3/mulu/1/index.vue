<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第一章</div>
      
     <div class="home" >
     
　　<p>那个男孩名叫圣地亚哥。暮色开始降临时，他与他的羊群来到了</p>一座废弃的古老教堂的门前。教堂屋顶很久前就已然塌落，在原先是圣器室的地方，已经长出了一棵巨大的埃及榕。 

男孩决定在这里过夜。他把所有的羊赶进残破的大门，随后又用几块木板挡在门上，以防夜里羊儿可能走失。这个地区没有狼，但有一次一只羊在夜里走失了，次日他花了整整一天的时间去寻找这只迷途的羊儿。 

他把自己的外衣铺在地上，然后躺了下来，把刚刚读完的一本书当作枕头来用。入睡之前，他提醒自己需要开始读一些更厚的书，读完这样的书要耗费更多的时间，而且夜里当作枕头也会更加舒适。 

当他醒来时天还没有亮。抬头向上望去，透过损毁了一半的屋顶，可以看到星星在闪烁。 

"真想再多睡一会儿，"他想道。刚刚做了一个梦，与上周所做的完全相同，而且也是在梦结束之前便醒了。 

他起身喝了一口酒，然后拿起牧羊拐杖，开始捅醒那些仍在睡觉的羊儿。他己经注意到，只要他一醒，大多数羊也同样开始醒来，仿佛有某种神秘的能量将他的生命与羊儿的生命联在了一起。两年来，他领着羊儿们走遍这块大地，寻找着水和食物。"它们已经太熟悉我了，所以知道我的作息时间。"他喃喃自语道。他思索了片刻，心想也可能恰恰相反，是他熟悉了羊儿们的作息时间。 

不过，仍有些羊儿要再过一会儿才醒。男孩一边呼唤着每只羊的名字，一边用牧羊杖一只接一只地捅醒它们。他一直相信这些羊能听懂他的话，所以有时他习惯于把书中的精彩片断读给它们听，或是向它们诉说一个原野上的牧羊人的孤寂与欢乐，还会把在经常路过的一些村庄所见到的新鲜事向它们做一番评论。 

但是最近两天，他的话题实际上只有一个:那个女孩。她是一个商人的女儿，住在距此地还有四天路程的那个村庄里。他只是去年到过那里一次。那个商人经营着一间纺织品商店，他总是喜欢让人当着他的面来剪羊毛，以免有人弄虚作假欺骗他。一位朋友介绍他去这家商店，牧羊少年就赶着羊群到了那里。 

"我需要卖一些羊毛。"男孩对商人说。 

商店里顾客盈门，商人要求牧羊少年等到快傍晚时再说。于是男孩便坐在商店门口碎石铺成的路面上，从搭褪里拿出了一本书。 
"那我就去当牧羊人。" 



</div>
<i-grid i-class="no-border">
    <i-grid-item @click="last" i-class="no-border">
        <i-grid-icon>
            <image src="http://img5.imgtn.bdimg.com/it/u=2179716670,977437141&fm=26&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label  >上一章</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="list" i-class="no-border">
        <i-grid-icon>
            <image src="https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2094031817,2842734087&fm=26&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label>目录</i-grid-label>
    </i-grid-item>
    <i-grid-item @click="next" i-class="no-border">
        <i-grid-icon>
            <image src="http://img1.imgtn.bdimg.com/it/u=2071479498,4142634719&fm=26&gp=0.jpg" />
        </i-grid-icon>
        <i-grid-label>下一章</i-grid-label>
    </i-grid-item>
    </i-grid>
  </div>
</template>

<script>
// Use Vuex
import store from './store'

export default {
  computed: {
    data () {
      return {
    
      }
    }
  },
  methods: {
    last(){
      wx.navigateTo({
        url: '/pages/book3/mulu/zixu/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/1/main'
      })
    }
  }
}
</script>

<style>
.no-border {
  border-width: 0pt;
}
.counter-warp {
  text-align: center;
  margin-top: 1px;
  background-color:burlywood
}
.home {
  display: inline-block;
  margin-left: 10px;
  margin-right: 10px;
  padding: 5px 10px;
  color: blue;
  border: 1px solid blue;
  text-align:left
}
.title{
  font-size: 80rpx;
  color: red;
  text-align: left
}
p {text-indent: 2em;}
</style>
