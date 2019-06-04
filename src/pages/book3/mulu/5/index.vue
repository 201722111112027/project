<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第五章</div>
      
     <div class="home" >
     
　　<p>他差一点就要讲出财宝的事，但最后还是决定闭口不谈</p>。如果说出来，这个阿拉伯人很可能会索要部分财宝，作为给他带路的报酬。男孩回想起老翁对他讲过的话:不要把还没有到手的东西许诺出去。 

"如果你行的话，我想让你带我到那里去。我可以付给你作为向导的报酬。" 

"那你想过怎么才能到达那里吗？" 

男孩发现酒吧主人正站在附近专心致志地听他们谈话。酒吧主人的出现使他感到不快。不过，他己经找到了一个向导，他不会失去这个机会。 

"你必须要穿越整个撒哈拉大沙漠，"刚来的小伙子说道，"要做到这一点我们必须要有钱。我想知道你是不是有足够的钱。" 

男孩认为这个问题很是奇怪。但他相信那位老翁，而老翁曾对他说过，当你渴望得到一件东西时，整个宇宙都会协力来帮助你。 

男孩从衣袋里取出钱，拿给那个小伙子看。酒吧主人凑了过来也看了看。酒吧主人与小伙子用阿拉伯语交谈了几句，前者显得十分气愤。 

"我们走吧，"小伙子对男孩说道，"他不愿意我们继续待在这里。" 

男孩松了一口气，站起身来付钱。但是酒吧主人拉住了他，开始不停地讲了起来。男孩身强力壮，不过，他正处身在一个陌生的国度。他的新朋友把酒店主人推到了一边，拉着男孩朝外走去。 

"他想要你的钱，"小伙子说道，"丹吉尔不同于非洲其他地方。这儿是一个港口，凡是港口总会有许多小偷。" 

男孩信任他的新朋友，是他在关键时刻帮助了自己。男孩掏出钱数了数。 



一看到两块宝石，他便感到了一阵极大的轻松。这两块宝石是他用六只羊换来的，是从纯金胸饰上取下来的。他可以把宝石卖掉，再买一张回程的船票。现在我可要变得更加机灵一点了，男孩边想边从搭褪取出宝石，然后把它们藏进了自己的口袋里面。此地是一个港口，这是那个小伙子告诉他的惟一真话，而一个港口总是到处都有小偷。 


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
        url: '/pages/book3/mulu/4/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/6/main'
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
