<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第九章</div>
      
     <div class="home" >
     
　　<p>宇宙存在着一种人人都能懂的语言，但是如今己被遗忘了</p>。除了其他东西之外，我正在寻找的就是 

这种宇宙语言。我正是因此才来到这里，因为我必须要找到一个懂得宇宙语言的人，他是一位炼金术士。" 

他们的谈话被货栈老板所打断。 

"你们两个真有运气，"胖胖的阿拉伯人说道，"今天下午就有一个商队出发去法尤姆。" 

"可我是要到埃及去。"男孩说道。 

"法尤姆就在埃及。"货栈老板说道，"你算什么阿拉伯人？" 

男孩说他是西班牙人。英国人甚感满意:男孩虽然穿着阿拉伯人的服装，但至少是个欧洲人。 

"他把预兆称作‘运气'。"胖胖的阿拉伯人走后英国人说道，"假如可能的话，我要撰写一部巨型的百科全书，谈谈‘运气'和‘巧合'这两个词。宇宙语言就是由这两个词写成的。" 

他对男孩说，他能与手里握着乌陵和土明的人相遇绝非是"巧合"。他问男孩是否也要去寻找那位炼金术士。 

"我是来寻找财宝的。"男孩说完便马上感到了后悔。不过英国人仿佛并末看重这件事。 

"从某种角度上看，我也是如此。"英国人说道。 

"我根本不知道什么是炼金术。"当货栈老板开始唤他们出去时男孩说道。 

"我是这支商队的领队。"一个蓄着长须长着一双黑眼睛的男人说道，"我掌握着商队每个人的生死大权，因为沙漠就像一个任性的女人，有时候会让男人发疯。" 

商队差不多有两百个人，还有两倍于人的牲畜——骆驼、马、驴、家禽。英国人有几只箱子，里面装满了书。人群中有妇女和儿童，还有一些腰里挎剑、肩上扛着长枪的男人。嘈杂声响成一片，领队不得不把他的话重复了好几遍，以便让所有的人都能听明白。 

"我们当中有各种各样的人，他们信奉着各不相同的神。我唯一信奉的神是真主安拉，我向他发誓，我将尽一切所能，把事情做到最好，以便再一次征服沙漠。我现在希望，你们每个人也向自己心底里所信奉的神发誓，无论在任何情况下都要服从我。在沙漠里，不服从就意味着死亡。" 


"马克图伯。"男孩说道，并回想起了水晶店店主。 


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
        url: '/pages/book3/mulu/8/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/10/main'
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
