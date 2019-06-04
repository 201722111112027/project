<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第四章</div>
      
     <div class="home" >
     
　　<p>"我离开了我的父亲，我的母亲，还有故乡的城堡。他们己经习惯了，而我也同样</p>如此。羊儿也会慢慢习惯我不在它们的身边。"男孩想道。 

男孩从上边望了一眼广场。小贩仍然在卖他的爆米花。一对年轻的情侣在刚才他与老翁谈话的长凳上坐下来，久久地亲吻。 

"那个小贩……"他自言自语道，却没有把话讲完，因为黎凡特风越刮越猛，他的脸感到了风的强劲。的确，这种风带来了摩尔人，但也同时带来了沙漠和头戴面纱的女人的气味，还带来了为寻求末知物、黄金、历险……以及金字塔而出发的男人们的汗味和梦想。男孩开始羡慕风的自由自在，并意识到他也能够如风一样。除了他自己，没有任何东西能够阻止他。羊群，商人的女儿，安达卢西亚的田野，都只是他迈向天命之路的一个个步伐而已。 

第二天中午，男孩带着六只羊和老翁见了面。 

"我很惊讶，"男孩说道，"我的朋友立刻买去了我的羊，还说他一生都梦想成为牧羊人。这是个好兆头。" 

"事情总是如此，"老翁说道，"我们把这称作为有助原则。如果你是第一次玩牌，几乎百分之百地会赢，这是新手的运气。" 

"为什么会这样呢？" 

"因为生活希望你去完成自己的天命。" 

老翁开始检查这六只羊，发现其中一只瘸了腿。男孩解释说这无关紧要，因为它是最聪明的一只羊，而且能产相当多的毛。 

"财宝在哪里呢？"他问道。 

"财宝在埃及，靠近金字塔。" 

男孩吃了一惊。解梦的老妇也是这样说的，但她没收取任何东西。 

"要想找到财宝，你必须随预兆而行。上帝为世上的每个人写出了他应该走的路，你只要读懂他为你所写的就行了。" 


牧羊少年默不作声。他己经理解了老国王讲的这个故事。一个牧羊人喜欢旅行，但永远不要忘记他的羊群。 


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
        url: '/pages/book3/mulu/3/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/5/main'
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
