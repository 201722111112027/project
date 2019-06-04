<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第八章</div>
      
     <div class="home" >
     
　　<p>但是羊儿却教过他一件更加非常重要的事情:世界上有一</p>种人人都能理解的语言，在让水晶店兴旺起来的整个那段时间里，男孩使用了这种语言。它是一种热情的语言，是以爱和意志所造就的事物的语言，是寻找某种你所希望或是你所相信之物的语言。丹吉尔对他而言己不再是一个陌生的城市，男孩感到，他能够用征服这个地方的同样方式去征服世界。 

"当你渴望得到某种东西时，整个宇宙都会协力使你实现自己的愿望。"老圣王曾经说过。 

但是老圣王没有说过会有人骗取钱财，没有说过会有无边无际的沙漠，也没有说过会有人知道自己的梦想却不希望去实现。老圣王没有说过金字塔只不过是一堆石头，谁都可以在自家的后院建造一个。而且他还忘记讲了，当你有了钱去买比原来还要多的羊群时，你就应该把它买下来。 

男孩拿起褡裢，把它与其他的包放在了一起，然后走下楼梯。老店主正在接待一对外国夫妇，同时还有另外两位顾客在店里转来转去，手持水晶杯喝茶。早晨这个时候能有这样的生意是蛮不错的。男孩从他所在的位置，第一次发现店主的头发很像老圣王的头发。他回忆起那位甜食商的微笑，那是他来到丹吉尔的第一天，当时他正无处可去和无东西可吃。甜食商的微笑也曾使他想到了老圣王。 

"仿佛老圣王从那里走过并留下了一个记号似的，"男孩想道。"他们一生中都从未见到过这位圣王。归根结底，老圣王说过，他总是为那些要完成自已天命的人而出现的。" 

男孩没有与水晶店店主辞行便出了门。他不想哭着与店主告别，因为这会被别人看到。但是他将会怀念整个这段日子，怀念他在这里所学到的所有美好的东西。他对自己更加充满信心，立志要征服世界。 

"可我现在却正要回到我己经熟悉了的田野，再次去牧羊。"他对自己的这一决定不再感到高兴。为实现一个理想我苦干了一年，而这一理想正分分秒秒地失去其重要性。也许是因为它并非是我的梦想。 

"谁知道是否像水晶店店主那样更好:永远不去麦加，而是靠要去那里的愿望来支撑生活。"然而男孩手里握着乌陵和土明，这两块宝石给他带来了老圣王的力量与意志。出于一种巧合 或者是一种预兆，男孩想道他来到了踏上非洲大陆第一天去过的那间酒吧。那个骗子己不在了，酒吧主人给他端上了一杯茶。

"我随时都可以重当牧羊人，"男孩想道。"我已经学会了牧羊，永远不会忘记羊儿是什么样子。但是也许我再也没有机会去埃及的金字塔。老撒冷王穿着一件金制的胸饰，知道我过去的一切，是一位真正的圣王，一位智慧的圣王。" 

他徒劳地寻找哲人石，为此而耗费了父亲留给他的部分遗产。他曾去过世界上那些最好的图书馆，并购买了最重要和最珍稀的有关炼金术的书籍。他在一本书上发现，在许多年前，曾有一位著名的阿拉伯炼金术士访问过欧洲。据说他已有两百多岁了，已经发现了哲人石和长命液。英国人被这个传说吸引住了，但假如不是他的一个从沙漠考古回来的朋友告诉他有位阿拉伯人具有特殊功能的话，那么这个传说就不过是个神话而已。 

"此人住在法尤姆绿洲，"他的朋友说道，"据说有两百岁了，能够将任何一种金属变为黄金。" 


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
        url: '/pages/book3/mulu/7/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/9/main'
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
