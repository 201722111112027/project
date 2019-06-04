<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第十五章</div>
      
     <div class="home" >
     
　　<p>"我不知道我能不能在沙漠中发现生命，"男孩想道</p>，"我还不了解沙漠。" 

男孩本想转身把自己的想法告诉炼金术士，但他对炼金术士望而生畏。两个人来到一片岩石地带，男孩曾在这里看到了天上的那两只老鹰，可现在此地却是一片沉寂，只有风声在响。 

"我无法在沙漠中发现生命，"男孩说道，"我知道生命是存在的，但我却不能发现它。" 

"生命吸引生命。"炼金术士回答道。 

男孩明白了，他立刻松开了马的缰绳，任马自由地在岩石和沙土上行进。炼金术士默默地跟在后面。男孩的马走了几乎半个小时，此刻他们已经看不到绿洲的椰枣树了，有挂在天空的一轮巨大的月亮和闪烁着银色光芒的岩石。突然，在男孩从未来过的一处地方，他注意到马停止了脚步。 

"这里存在着生命。"男孩对炼金术士说道，"我不熟悉沙漠的语言，但是我的马熟悉生命的语言。" 

\奇\两个人下了马。炼金术士一言不发，开始一边打量岩石一边慢慢地行进。突然，他停下脚步，十分小心地弯下腰来。岩石间的地面上有一个洞，炼金术士把手伸了进去，接着直至肩膀的整个胳膊都伸了进去。洞里有个东西在动，炼金术士的眼睛——男孩只能看到他的眼睛——由于用力和紧张而收缩。他的胳膊似乎正在与洞里面的东西进行搏斗。只见炼金术士一跳——令男孩大吃一惊——，抽出了胳膊，并立刻站立起来。他的手紧紧抓住了一条蛇的尾巴。 

\书\男孩也跳了一下，只不过是向后而去。那条蛇在不停地挣扎，发出的咝咝响声打破了沙漠的沉寂。这是一条眼睛蛇，它的毒液能在短短的几分钟内致人于死命。 

"小心它的毒液，"男孩想道。不过，炼金术士刚才曾经把手伸进过洞里，大概已经被咬过了，然而他的面部表情却很平静。"炼金术士己有两百岁了。"英国人曾经说过。他应该知道如何对付沙漠里的蛇。 

男孩看到炼金术士来到马的身边，抽出长长的弯月形剑，用它在地上画了一个圆圈，然后把蛇放进圈的中央，蛇立刻安静下来。 

"你放心好了，"炼金术士说道，"它不会出这个圈的。你发现了沙漠中的生命，这正是我所需要的预兆。" 

"为什么这竟如此重要呢？" 

"因为金字塔被沙漠所包围。" 

"我将与你同行。"男孩说道，并立刻感到内心一片宁静。 

"明天太阳升起之前我们动身。"这便是炼金术士的唯一回答。

不去想过去的事情是很难做到的。几乎总是一成不变的沙漠景象常使人充满幻觉。
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
        url: '/pages/book3/mulu/14/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/16/main'
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
