<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第十八章</div>
      
     <div class="home" >
     
　　<p>阿拉伯人不声不响地接了过去。这些金币可以</p>购买许多武器。 

"炼金术士是干什么的?"最后他问道。 

"炼金术士通晓自然和世界的奥秘，假如他愿意的话，只要借助风的力量就能把这个营地摧毁。" 

那些人笑了起来。他们熟知战争的力量，风并不能阻止一次致命的攻击。然而在他们每个人的胸膛，心脏都加快了跳动。他们是沙漠的男人，对巫师充满恐惧。 

"我倒想看一看。"指挥官说道。 

"我们需要三天的时间。"炼金术士回答说，"他会把自己变成风，目的不过是要展示一下他所掌握的功能的威力。倘若他做不到的话，我们将卑躬屈膝地为贵部落的荣誉而贡献我们的生命。" 

"你用不着把己经属于我的东西贡献给我。"指挥官趾高气扬地说道。 

不过，他同意给他们三天的时间。 

男孩吓得全身不能动弹。炼金术士抓住他的胳膊，把他架出了帐篷。 

"不能让他们察觉出你的恐惧。"炼金术士说道，"他们都是些勇敢的人，鄙视胆小鬼。" 

但是男孩却说不出活来。过了一段时间，当他们行走到营地中央时，男孩才终于能够开口讲话了。没有必要把他们关押起来，阿拉伯人仅仅牵走了他们的马。世界再次展示了它的多种语言:此前，沙漠还是一片自由和无根的天地，现在却成了一道无法逾越的大墙。 

"你把我所有的钱全给了他们!"男孩说道，"这是我整整一生挣来的!" 
"你在干什么？" 

"喂我的猎鹰。" 
风十分傲慢，男孩的话刺激了它。于是它开始更猛烈地刮了起来，扬起了沙漠的沙粒。然而最终风不得不承认，尽管它跑遍了整个世界，也不知道如何把人变成风。它不了解爱。 

"当我在世界各地漫游时，发现许多人谈起爱的时候都仰望着天空，"风说道，它因为不得不承认自己的局限性而怒气冲冲，"也许最好是问问天空。"
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
        url: '/pages/book3/mulu/17/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/19/main'
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
