<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第二十章</div>
      
     <div class="home" >
     
　　<p>他们骑上了各自的马。 

"科普特"原意为埃及人，是阿拉伯人于七世纪</p>中叶进人埃及时对埃及 

原有居民的称呼。后专指信仰科普特派基督教的人。 

"我想给你讲一个关于梦的故事。"炼金术士说道。 

男孩把他的马靠近了炼金术士。 

"在古代罗马提比略皇帝当政时代，一个心地十分善良的人有两个儿子。一个是军人，入伍时被派往帝国最边远的地区。另一个是诗人，他用美丽的诗句迷住了整个罗马。 

"一天夜里，老人做了一个梦，一位天使前来对他说，他的一个儿子的话语将世世代代流传下去，为全世界的人所熟知和反复吟诵。那天夜里老人醒来后感激涕零，因为生活十分慷慨，向他揭示了任何一位父亲知道后都会感到自豪的一件事情。 

"不久之后，老人在试图抢救一个行将被芋轮压过的小孩时死去。由于他一生中行为端正，无可指摘，所以就直接去了天堂，并遇到了在他梦中出现的那位天使。 

"你一直是个好人，"天使对他说，"活着的时候充满爱心，死得也很尊严。现在我可以实现你的任何愿望。" 

"‘生活对我也一直很好，'老人回答说，‘当你出现在我的梦中时，我感到我的所有努力都被证明是正确的。因为我儿子的诗句将在后世的人们之间流传。我为自己提不出任何要求，但是所有的父亲都会为看到自己的儿子享有盛名而感到骄傲。儿子小的时候做父亲的曾养育过他，儿子年轻的时候做父亲的曾教育过他。我希望到遥远的未来去，看看我儿子留下的话语。’" 

"天使摸摸老人的肩膀，他们俩便一起被投向一个遥远的未来。他们置身于一个广阔无根的地方，有数以千计的人在讲着一种奇怪的语言。 

"老人高兴地哭了。 
男孩艰难地站立起来，再次朝金字塔望去。金字塔在朝他微笑，而男孩也以微笑回报，心灵充满了幸福。
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
        url: '/pages/book3/mulu/19/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/21/main'
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
