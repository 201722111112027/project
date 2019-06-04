<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第三章</div>
      
     <div class="home" >
     
　　<p>"那我们就面临一个难题了。如果你认为你有足够多的羊，我就</p>无法帮助你了。" 

男孩不高兴了。他并没有请求帮助，相反是老翁跟他要酒喝，找话谈，翻阅他的书。 

"请把书还给我。"男孩说道，"我要去赶我的羊群上路了。" 

"把你十分之一的羊儿给我，"老人说道，"我就教你如何找到宝藏的地方。" 

男孩于是又想起了他的梦，突然间一切都变得清清楚楚。老妇没有收取他一文钱，但这个老翁——也许是她的丈夫——，却以提供莫须有的信息为交换条件，想骗取他更多的钱。老翁大概也是个吉卜赛人。 

不等男孩开口，老翁便俯下身子，拿起一根木棍，开始在广场的沙地上写了起来。俯身时，他怀里的一个什么东西闪烁了一下，放射出的光芒如此强烈，几乎使男孩什么都看不见了。老翁以一个他这种年纪不该有的极快动作，又用罩袍将那个发光物遮盖住了。男孩的视力恢复了常态，看清了老翁所写的东西。 

在这个小城主广场的沙地上，男孩读到了自己父母亲的名字，读到了直至此刻为止他走过的人生历程，童年的玩耍，神学院的寒夜。他还读到了那个商人的女儿的名字，这是男孩过去一直不知道的。有些事情他从未向任何人讲过，比如有一天他曾偷出父亲的枪打死过鹿，还有他的第一次独自的性体验，也竟然都写在了沙地上。 

"我是撒冷之王。"老翁说道。 

"一个国王为什么要和一个牧羊人交谈呢？"男孩羞愧而又极为敬畏地间道。 

"有几个原因。但我要说的是，最重要的是你已具备能力履行你的天命。" 

男孩不懂得什么是天命。 

"天命就是你一直总希望去做的事情。所有的人在刚步人青年时代时，都知道自己的天命是什么。 

"在生命的那一时刻，一切都清清楚楚，一切都是可能的，人们敢于梦想，敢于渴望他们喜欢见到的一切发生在自己的生活之中。然而，随着时光的流逝，一种神秘的力量开始试图证明，实现天命是不可能的。" 



老翁翻阅着那本书，漫不经心地读着其中的一页。男孩等待了片刻，然后就以老翁打断他的同样方式也打断了老翁的阅读。 


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
        url: '/pages/book3/mulu/2/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/4/main'
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
