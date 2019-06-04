<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第十七章</div>
      
     <div class="home" >
     
　　<p>从那一天起，男孩理解了自己的心灵。他请求心灵永远都不要离开</p>他。他还请求，当他远离自己的梦想时，心灵要在胸膛加快跳动，发出警报的信号。男孩发誓，只要一听到这个信号，便会听从它的指引。 

那天晚上，男孩把这一切都告诉了炼金术士。炼金术士明白，男孩的心灵己返回世界灵魂。 

"现在我该怎么做呢？"男孩问道。 

"朝金字塔方向前进。"炼金术士说道，"你要继续留意预兆。你的心灵己经能够为你指出财宝在何处了。" 

"这就是我所需要知道的吗？" 

"不。"炼金术士回答说，"你需要知道的事情如下: 

"在实现一个梦想之前，世界灵魂总是决定要对寻梦者一路所学到的一切加以检测。它所以这样做并非因为它居心不良，而是让我们与梦一起，也能够掌握在寻梦过程中所学习到的知识。这是多数人会放弃的一个时刻。在沙漠的语言中，我们把这称之为‘渴死在椰枣树己经出现在地平线上之时’。 

"每一次寻梦都以创始者的运气开始，又总以对征服者的考验结束。" 

男孩回想起故乡的一句古老的谚语:最黑暗的时刻出现在黎明之前。 

翌日，第一个具体的危险信号出现了。三名部落战士走近他们，询问男孩和炼金术士到这里来干什么。 

"我是带着猎鹰来狩猎的。"炼金术士回答道。 

"我们需要对你们进行搜查，看看你们是不是带着武器。"其中的一位战士说道。 

炼金术士缓缓地下了马，男孩也同样如此。 

"你带着这么多钱干什么?"搜查男孩钱袋的战士问道。 

"为了能到达埃及。"男孩回答说。 

搜查炼金术士的战士发现了一个装满液体的小水晶瓶，还有一个比鸡蛋略大一点的黄色玻璃蛋。 

"这是些什么东西？"战士问道。 
"他带来了钱想献给你们部落。"不等男孩开口，炼金术士便抢先回答说，接着就拿过男孩的钱袋，把金币交给了指挥官。
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
        url: '/pages/book3/mulu/16/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/18/main'
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
