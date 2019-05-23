<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第二十一章</div>
      
     <div class="home" >
     
　　<p>他找到了财宝。 

男孩名叫圣地亚哥。暮色儿乎已耍降临时，他来到</p>了那座废弃的小教堂。埃及榕依然生长在圣器室里，透过毁了一半的屋顶依然能看到群星。男孩回忆起，有一次他曾领着羊群来到这里，除了做梦之外那是一个宁静的夜晚。 

现在他又来到了这里，不是领着羊群，而是带来了一把铁锹。 

他久久地凝视着天空。后来他从褪搭里取出一瓶酒喝了起来。他回忆起在沙漠的那个夜晚，当时他也是望着群星，与炼金术士一起喝酒。他想起了他走过的许多道路，还有上帝为他指出财宝的奇异方式。假如当初他不相信两次做过的同一个梦，就不会遇到那个吉卜赛女人、圣王、小偷以及……"是啊，那是个极长的名单，但是道路已被种种预兆写定，因此我不会走错。"他自言自语道。 

男孩不知不觉地睡着了，当他醒来时，太阳已经升起很高了。于是他开始在埃及榕的根部挖掘起来。 

"老巫师，"男孩想道，"你无所不知，甚至给我留下了一块金子，好让我能回到这个教堂来。看到我穿着破烂衣衫回去时，那位修道士笑了。难道你就不能让我免受这次罪吗？" 

"不能。"男孩听到风声说道，"如果我事先告诉你，你就不会看到金字塔。它们非常壮丽，你不这样认为吗？" 

这是炼金术士的声音。男孩微微笑了，接着又继续挖掘。半个小时之后，铁锹碰到了某个坚硬的东西。一个小时之后，男孩眼前出现了一个装满西班牙古金币的箱子。箱子里还有宝石、装饰着红白两种颜色羽毛的金制面具和镶嵌着钻石的石制偶像。这是一次征服的战利品，国家早就把它们遗忘了，而征服者本人也忘记了将其告诉他的子女们。 

男孩从褪搭里取出乌陵和土明。他只使用过一次这两块宝石，是某个早晨在一个市场上。生活及其道路总是充满着预兆。 

男孩把乌陵和土明收进宝箱里。这也是他的财宝的一部分，因为它们能使他回想起那位他将永远再也无法见到的老圣王。 

"生活对追随自己天命之人是慷慨的，"男孩想道。此刻他回想起他必须要到塔里法去，把全部财宝的十分之一送给那位吉卜赛女人。"吉卜赛人是何等地聪明啊，"男孩想道。也许是这样的，因为他们到处旅行。 

风又重新刮了起来。是来自非洲的黎凡特风。它没有带来沙漠的气息，也没有带来摩尔人人侵的威胁。相反，它带来了一股他非常熟悉的香味，还有一个吻的响声——这个吻缓缓地、缓缓地而来，直到停在他的双唇上。 

男孩微微笑了。这是她第一次这样做。 

"我来了，法蒂玛。"他说道。 

（全书完） 
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
        url: '/pages/book1/pfsj/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book1/2/main'
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
