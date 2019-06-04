<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第十六章</div>
      
     <div class="home" >
     
　　<p>男孩依然能看到椰枣树、水井以及他所爱着的那个女人</p>的相貌。他看到了正在实验室里的英国人，还有那位赶驼人。赶驼人是位导师，但他自己却并不知道。"也许炼金术士从未恋爱过，"男孩想道。 

炼金术士骑马走在前头，肩上站着猎鹰。猎鹰十分精通沙漠的语言，当他们停下来时，猎鹰便离开炼金术士的肩头，飞去寻找食物。第一天它带回一只兔子，第二天带回两只鸟。 

入夜之后，他们铺开毛毯，并不点燃篝火。沙漠的夜晚十分寒冷，且随着天空的月亮开始缩小而变得黑暗。他们默默无语地走了一个星期，只就采取必要的戒备以避开部落之间的战争交谈过几句。战争仍在继续，有时风会带来血的淡淡的甜味。附近曾发生过一场战斗，风提醒男孩预兆语言的存在，它随时准备显现出男孩的眼睛无法看到的东西。 

第七天的旅程结束时，炼金术士决定要比往常早一些露营。猎鹰飞出去寻找猎物，炼金术士取出旅行水壶递给了男孩。 

"现在你几乎到达旅程的终点了，"炼金术士说道，"我祝贺你追随了自己的天命。" 

"你一直默默无语地为我领路，"男孩说道，"我本以为你将把你所会的东西教给我。前一段时间，我在沙漠中与一个男人在一起，他带有一些炼金术的书籍，可我什么也没有学到。" 

"只有一种学到的方式，"炼金术士回答说，"那就是通过行动。你所需要学到的一切，旅行都已教会了你，现在就只差一件事情了。" 

男孩想知道是什么，但是炼金术士的眼睛却注视着地平线，等候着猎鹰的归来。 

"为什么人们把你叫作炼金术士？" 

"因为我是炼金术士。" 

"其他的炼金术士们炼金却没有成功，他们错在什么地方呢？" 

"他们只是炼金而已，"炼金术士回答道，"他们寻找自己天命中的财宝，却不希望履行自己的天命。" 

"我还需要学会什么呢？"男孩问道。 
"因为在这种情况下，心灵会忍受更大的痛苦，而心灵不喜欢忍受痛苦。"
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
        url: '/pages/book3/mulu/15/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/17/main'
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
