<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第十二章</div>
      
     <div class="home" >
     
　　<p>当这样的两个人相遇而且目光交汇在一起时，</p>所有的过去和所有的未来便都失去了其重要性，存在的只有这一时刻本身，还有不可思议地确信太阳底下所有的事情都是由同一只手写定的。这是一只唤醒爱情的手，是为在太阳底下工作、休息和寻找财宝的人们铸造了同样灵魂的一只手，如果没有这一切，人类的梦想便没有任何意义。 

"马克图伯，"男孩想道。 

英国人从坐着的地方站了起来，摇了摇男孩。 

"快啊，快问她呀!" 

男孩靠近少女，少女又微微一笑，男孩也微微一笑。 

"你叫什么名字?"他问道。 

"我叫法蒂玛。"少女望着地面答道。 

"我们那个地方有一些女人也叫这个名字。" 

"这是先知的女儿名字，"法蒂玛说道，"战士们把它带到了你们那里。" 

" 

娇弱的少女讲到战士时颇为骄傲。在一旁的英国人一个劲地催促，于是男孩问起此地是否有个能医治百病的男人。 

"这个人通晓世上所有秘密，能与沙漠的精灵交谈。"少女说道。 

精灵便是魔鬼。少女指了指南方，那位奇人就住在那边。 

把水罐装满水之后少女就走了。英国人也走了，去找那位炼金术士。男孩在井边坐了很长的时间，他明白了某一天黎凡特风留在他脸上的正是这位少女的芳香，明白了甚至在知道她的存在之前就已经爱上了她，还明白了凭借他对少女的爱便能找到世界上所有的财宝。 

先知系指伊斯兰教创始人穆罕默德(约570-632)，他有个女儿名叫法蒂玛。[/face] 

第二天，男孩又来到井边，等候着少女的出现。令他吃惊的是，他在那里遇到了英国人正在第一次凝视沙漠。 

"我等了一个下午和一个晚上，"英国人说道，"直到最初的星星升起时他才露面。我向他讲述了我正在寻求什么，于是他问我是否已经把铅变成了金。我对他说，这正是我想要学会的东西。 

"他让我试一试。去试试吧，这就是他对我所说的一切。" 

男孩没有讲话。英国人长途跋涉，所听到的却是他已经知道的东西。男孩由此回想起，出于同样的原因，他给了老圣王六只羊。 

"那就去试试吧。"他对英国人说道。 

"这就是我正要去做的事，就从现在开始。" 

英国人走后不久，法蒂玛就肩扛水罐前来汲水。 

"我来只是想告诉你一件事情，"男孩说道，"我想让你成为我的妻子。我爱你。" 

少女把水罐里的水放掉了。 

"我每天都会到这里来等你。我穿越沙漠，想寻找到金字塔附近的一处财宝。对我来说，战争曾是一场灾难，现在却成了一种福音，因为它让我来到了你的身边。" 

"战争总有一天会结束的。"少女说道。 

男孩望了望绿洲里的椰枣树。他曾是个牧羊人，而这里有许多羊。法蒂玛比财宝更重要。 

"战士们要寻找他们的财宝，"少女说道，仿佛猜出了男孩的想法，"沙漠的女人为她们的战士们感到骄傲。"随后她重新将水罐装满，接着便离去了。 


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
        url: '/pages/book3/mulu/11/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/13/main'
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
