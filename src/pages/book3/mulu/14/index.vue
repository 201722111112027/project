<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第十四章</div>
      
     <div class="home" >
     
　　<p>但是在死去之前，他已经跨越了海峡，在一家水晶店打</p>过工，了解了沙漠的沉寂，见识了法蒂玛的那双眼睛。从很久以前离开家乡之后起，他的每一天都过紧张而充实。哪怕是明天行将死去，他的眼睛所见到的事物也比其他牧羊人的要多得多。男孩为此而感到骄傲。 

突然他听到一声巨响，接着便被一阵他从未见过的狂风猛地吹倒在地。尘埃四起，几乎遮住了月亮。一匹巨大的白马扬起前蹄直立在他的面前，发出了一声吓人的嘶鸣。 

男孩儿乎看不清正在发生的事情，但是当尘埃稍稍落定之后，他却感到了一种过去从未有过的恐惧。一个全身着黑装的骑手跨坐在白马之上，左肩上立着一只猎鹰，头上缠着裹 头布，一条头巾遮住了整个的脸，只露出两只眼晴。看上去他好像是沙漠里传递消息的信使，但他的外表要比男孩一生中认识的所有人都更加强壮。 

古怪的骑手从束在马鞍上的剑鞘里抽出一把巨大的弓形长剑，钢刃在月光的映照下闪闪发光。 

"是谁竟敢解读老鹰飞翔的预兆？”骑手问道，声音如此洪亮，仿佛在绿洲的五万棵椰枣树中间激起了回响。 "我敢。"男孩说道，并立刻回忆起圣徒圣地亚哥?马塔莫罗斯的画像来:圣徒骑在他的白马上，一些异教徒倒在马蹄之下。眼前的情景恰恰正是如此，只不过位置颠倒了过来。 

"我敢。"男孩又说了一遍，然后便低下头，等候着承接剑的刺击。 

"许多人的生命将会被拯救，因为你们不懂世界灵魂。" 

然而剑并没有飞快地刺下来。那个怪人的手慢慢地向下移动，直至剑锋碰到男孩的前额。剑锋无比锐利，男孩的前额流出了一滴血。 

骑手全然地一动不动。男孩也同样如此。男孩连一分钟也没有想过要逃走，内心深处涌起了一种奇怪的快意:他将为自己的天命而死。还为法蒂玛而死。总之，预兆是真实的。敌人就在眼前，故而他无需担心死去，因为存在着世界灵魂，很快他就将成为它的一部分。明天敌人也将同样成为它的一个部分。 

那个怪人只是继续将剑抵在男孩的前额。 

"为什么你要解读老鹰飞翔的预兆？“ 

"我只读了老鹰想要告诉我的东西。它们想拯救绿洲，你们将必死无疑。绿洲的人要比你们多。" 

剑继续抵在男孩的前额。 

"你是什么人，竟要改变安拉的旨意？” 

"安拉创造了军队，也创造了鸟类。安拉向我展示了鸟类的语言。所有的一切都是同一只手写定的。"男孩说道，他想起了赶驼人的话。 
在依然明亮的月光照耀下，两个人开始沿着沙地前行。
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
        url: '/pages/book3/mulu/13/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/15/main'
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
