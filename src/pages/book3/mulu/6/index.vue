<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第六章</div>
      
     <div class="home" >
     
　　<p>甜食商的笑容使男孩回想起他遇到的那位老翁、那</p>位神奇的圣王的某些事情。"这个甜食商不制作甜食，因为他想外出旅行，或是因为他想和一个商人的女儿结婚。这个甜食商制作甜食，因为他喜欢这个工作。"男孩想道，并发现他也可以做出老翁能做的同样的事情:知道一个人是走近还是远离他的天命。只要观察一下此人就行了。"这很容易，而我过去却从没有察觉到这一点。"男孩想道。 

两个人搭好货摊后，甜食商把他制作的第一份甜食递给了男孩。男孩吃得饱饱的，道过谢之后便上路了。当已经离开那里一会儿之后，他突然回想起，架设摊位时，他们两人一个讲的是阿拉伯语，另一个讲的是西班牙语。 

但是他们完全能相互理解。 

"一定存在着一种超越言词的语言，"男孩想道，"我己经从羊儿那里体验过这一点，现在又从人那里体验到了。" 

他正在掌握某些新的东西。有些东西他也曾经历过，但仍然是新的，因为当时虽然经历了却未曾察觉到。他所以未曾察觉到，乃是因为他己习惯了这些东西。"假如我学会理解这种没有言词的语言，我就能理解这个世界。"男孩想道。 

"万物为一。"那位老翁曾经说道。 

男孩决定不急不忙、不焦不虑地沿丹吉尔狭窄的街道而行，因为只有这样，他才能够察觉到预兆。这需要极大的耐心，但此乃一个牧羊人学会的第一种品德。他又一次发现，他在这个陌生的世界里，恰恰正运用着羊儿教给他的那些知识。 

"万物为一。"那位老翁曾经说道。 

看到天亮了，水晶店店主感到了每日清晨都要经历的同样烦恼。商店位于一个斜坡的坡顶，很少有顾客由此经过，他在这同一个地方一呆几乎快三十年了。现在要想有任何改变都为时晚矣。他一生学会的惟一事情就是买卖水晶制品。从前曾有过一段时间，很多人都知道他的商店，有阿拉伯商人，有法国和英国的地质学家，还有口袋里总是有钱的德国士兵。在那个时代，出售水晶制品很是赚钱，他曾设想过如何成为一个富翁，如何在年迈时得到漂亮的女人。 

后来，好时光一去而不复返，城市也同样如此。休达市的发展超过了丹吉尔市，商机随之发生了转向。邻居们先后搬走了，斜坡地只留下了少数几家商店。谁也不会为逛这儿家商店而爬上斜坡。 

但是水晶店店主却别无选择。他从事水晶制品生意三十年了，要改做其他事情己为时太晚。 

整个上午，他都望着街道上少数行人的走动。这种情形己有许多年了，他都能知道每位行人由此路过的时间。还差几分钟就要吃午饭的时候，一个外国男孩在他的橱窗前停了下来。男孩的服装同常人一样，可水晶店店主那双经验丰富的眼睛却断定此人没钱。尽管如此，水晶店店主还是决定略等片刻，等男孩离去后再吃午饭。 

商店门口的一个招牌说明这里可以使用几种语言。男孩看到一个男人出现在柜台后面。 

"如果你愿意的话，我可以把这些杯子擦干净。"男孩说道，"它们现在的这副样子，任何一个顾客也不会想购买。" 

男人看着男孩什么话也没讲。 

"反过来，你要管我一顿饭。" 



然而店主却理解了男孩所说的话。男孩来到他的商店这一简单的事实就是个预兆，随着时间的推移，随着钱柜里的钱越来越多，他对雇用了一个西班牙人一点都不后悔，尽管男孩所挣的钱比其应该得到的要多。当初他一直认为生意不会发生什么变化，所以答应给男孩的佣金甚高，而且他的直觉告诉他，男孩很快就会回去牧羊。 


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
        url: '/pages/book3/mulu/5/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/7/main'
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
