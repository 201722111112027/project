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
