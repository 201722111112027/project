<template>
  <div class="counter-warp" >
                   <div text-align="center">第二十九章</div>
                   <div class="home">
  <p>孙少安其实并没有任何可办的事。</p>！

他立刻又把自己从孩子的状态变成大人的状态，对父亲说：“爸爸，你不要难受。我什么事也没！我只是一时心里闷得不行，想一个人消散一会。你放心！我不会做什么出边事；我才二十三，还没活人哩，怎么可能往绝路上走呢？你想想，我从十三岁开始和你一块撑扶这个家，我怎么能丢下这一群人呢？你不要哭了，爸爸。你放心！我的心一点也没松，我还会象往常一样打起精神来的。我年轻，苦一点也没什么。咱们受苦人，光景日月就这么个过法，一辈子三灾六难总是免不了的。也许世事总会有个转变，要是天年再好一点，咱们的光景会翻起来的。再说，少平和兰香也快大了，咱两个一定把他们的书供到头。咱家七老八小，就看咱两个撑扶这光景哩。你不要灰心，门里门外的大事总有我承担哩……”

孙玉厚听了儿子的一番话，就难为情地用手掌把脸上的泪水和鼻涕揩掉，在鞋帮子上擦了擦手，然后沉痛地说：“爸爸对不起你。爸爸一辈子没本事，没把你的书供成，还叫你回来劳了动。受苦不说，你这么大了，爸爸连个媳妇也给你娶不回来。爸爸心里象猫爪子抓一样，死不能死，活不能活啊！”

少安重新点着一支旱烟卷，对父亲说：“我的婚事你不要熬煎。我年龄还不算大。就是年龄大了，我不相信我就打光棍呀。到时我自个儿找一个。只要财礼少，我不挑拣人。女方不嫌咱家穷，能和咱们一块过光景就行了。”“你也不小了，得看着给你瞅个媳妇。只要有你合心的，财礼多少不怕，咱们打闹着借，慢慢再还。我现在还能出山哩，少平高中也快念完了，咱父子三个熬上几年，就会把帐债还完的。”

“我不想掏这些财礼。财礼重的人家我不会娶。咱们不能再欠帐债，这样一辈子也翻不起来！”

“可是天下没有不要钱的人家啊！”

“慢慢碰吧……爸爸，天不早了，咱们回去吧！家里人一定心焦得不知咱两个出了什么事。”

于是，孙少安父子俩就站起来，拍了拍身上的土，出了高粱地，在月光下顺着公路回家去了……
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
        url: '/pages/book1/21/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book1/23/main'
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
  text-align:"left"
}
p {text-indent: 2em;}
</style>