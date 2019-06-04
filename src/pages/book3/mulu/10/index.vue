<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第十章</div>
      
     <div class="home" >
     
　　<p>赶驼人走后男孩对英国人说道，"商队绕了许多圈子，却始终把同一</p>个地方作为方向。" 

"你应该多读些了解世界的图书，"英国人回答道，"图书与商队是一模一样的。" 

由人和牲畜组成的庞大商队开始加速前进。过去人们习惯于在晚间围着簧火聊天，现在不仅白天都沉默不语，连晚间也都开始闭口无言了。有一天领队决定，为了不引起外界对商队的注意，夜间不再点燃簧火。 

为了抵御夜间的寒冷，人们用牲畜围成了一个圆圈，所有的人都睡在圆圈中央。领队还在商队周围安排了武装哨兵。 

一天夜里，英国人睡不着觉。他叫醒了男孩，两个人开始沿着宿营地四周的沙丘散步。一轮圆月当空，男孩向英国人讲述了自己的经历。 

英国人被水晶店的故事深深吸引，自从男孩开始在那里工作之后水晶店的生意便蒸蒸日上。 

"这便是推动一切事物的基点，"英国人说道，"在炼金术中被称作世界灵魂。当你全心全意期望得到某种东西时，你就更加接近了世界灵魂。它总是一种积极向上的力量。" 

他还说，这不只是人类独有的一种天赋，世上万物也都具有灵魂，无论是矿物、植物、动物，甚至一个简单的念头，都莫不如此。 

"地球上所有的事物都一直在变化，因为地球是有生命的，也具有灵魂。我们是这一灵魂的组成部分，可却极少知道它总是在帮我们的忙。不过，你应该明白，在水晶店里，甚至连那些水晶杯都在为你的成功而协力相助。" 

男孩望着圆月和白沙，半晌没有讲话。 

"我一直看着商队在沙漠中行进，"男孩终于开口道，"发现商队与沙漠讲着同一种语言，因此沙漠才允许商队通过自己。沙漠将检验商队迈出的每一步，以便观察它是否与自己完全协调一致。如果商队做到了与沙漠完全协调一致，它就必将到达绿洲。 

"假如我们之中的一个人以十足的勇气来到这里，但却不懂得这种语言，那么在第一天他就会死去。" 

两个人一起继续望着圆月。 

"这就是预兆的神奇之处。"男孩接着说道，"我目睹了向导们如何看懂沙漠的预兆，商队的灵魂如何与沙漠的灵魂对话。" 

过了一段时间，英国人开口了。 

"我需要多注意观察商队。"他终于说道。 

"我需要读读你的书。男孩说道。 
"这些书是什么时候写成的？"男孩问道。 

"许多世纪之前。" 

"那个时代还没有发明印刷，"男孩争辩说，"没有办法让所有的人都了解炼金术。为什么这种语言如此古怪，并且配上插图呢？" 


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
        url: '/pages/book3/mulu/9/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/11/main'
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
