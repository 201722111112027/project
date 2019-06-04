<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第二章</div>
      
     <div class="home" >
     
　　<p>现在，当老妇握着他的双手时，原有的那种恐惧重又出现了。 </p>

"但是这里有圣心耶酥像。"男孩想道，竭力使自己更镇静一些。他不想让自己的双手发抖，不想让老妇察觉出他的恐惧。他暗自默诵了一遍天父经。 

"真有意思。"老妇望着男孩的双手说道，然后便又沉默不语。 [网罗电子书：www.WRbook.com] 

男孩紧张起来，双手不由自主地开始抖动，老妇察觉到了这一点。男孩赶紧把手抽了回来。 

"我不是来看手相的。"男孩说道，已经后悔自己走进了那个家。他想了片刻，觉得最好是交钱走人，哪怕是一无所获。他太看重一个做过两遍的梦了。 

"你是来找我解梦的，"老妇说道，"梦是上帝的语言。如果上帝使用的是世俗的语言，我就能够做出解释。但是如果他使用的是心灵的语言，那就只有你自己才能够理解。不管怎样我都要收费。" 

又是一个诡计，男孩想道。但是他决定冒险。一个牧羊人总要遇上碰到狼或是干旱的风险，正是这一点才使牧羊人的生涯更富于刺激性。 

"我接连两次做了同一个梦，"男孩说道，"梦见我在田野放羊时来了一个小孩，他开始和羊儿们玩耍。我不喜欢有人逗弄我的羊，它们害怕生人。不过，孩子们总能逗弄它们又不使它们受到惊吓。我不知道为什么会这样，不明白羊儿怎么会识别人的年龄大小。" 

"回到你的梦上来，"老妇说道，"我的火上还放着锅，况且你只有不多的钱，不能占用我的全部时间。" 

"那个小孩继续和羊儿玩耍了一阵儿，"男孩接着说道，显得有些不自在，"突然，他抓起我的双手，把我一直带到了埃及的金字塔。" 

男孩停顿了片刻，想看看老妇是否知道埃及的金字塔是什么，但是老妇没有开口。 

"在埃及的金字塔，"男孩慢慢地讲出这几个字，以使老妇能够听明白，"那个小孩对我说:。如果你来到这里，就会找到一批埋藏着的财宝。'正当他要指给我宝藏的具体位置时，我就醒了。两次都是这样。" 

老妇又沉默了一会儿，然后再次拿起男孩的双手仔细地研究了一番。 

"现在我不收取你任何费用，"老妇说道，"但是如果你找到了宝藏，我想要其中的十分之一。" 

男孩高兴地笑了。因为事关一个宝藏之梦的缘故，他就可以省下他不多的钱来了。老妇准是个吉卜赛人——吉卜赛人都像驴一样地蠢。 

"那你就为我解梦吧。"男孩说。 

"你先要发誓，发誓将你的财宝的十分之一给我，作为我为你解梦的酬金。" 


　　
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
        url: '/pages/book3/mulu/1/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/3/main'
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
