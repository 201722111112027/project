<template>
  <div class="counter-warp">
     <div class="title" text-align="left">牧羊少年奇幻之旅</div>
     <div text-align="center">第十三章</div>
      
     <div class="home" >
     
　　<p>那位赶驼人坐在一棵椰枣树下，也在望着日落的</p>景象。他看到男孩从一个沙丘后面走了过来。 

"有一支部队正接近绿洲，"男孩说道，"我产生过一个幻景。 " 

"沙漠总是让一个人的心灵充满幻景。"赶驼人回答说。 

男孩向赶驼人讲述了两只老鹰的事:当他突然深人世界灵魂之时看到了它们的飞翔。 

赶驼人平静下来。他明白了男孩在说些什么。他知道，地球上任何一件东西都可以讲出万物的来龙去脉。无论是谁，如果把书随便翻到哪一页，或是观看人们的手相，或是通过扑克牌，或是通过观察鸟儿的飞翔，或是通过任何其他手段，都总会找到与自己正经历的事情相关的某种联系。其实并非是这些事物能够显示任何东西，而是那些观察这些事物的人发现了深入世界灵魂的方法。 

沙漠到处都有这样的人，他们轻而易举地就能深入世界灵魂，并以此为生。这些人被称为占卜师，妇女和老人都对他们十分敬畏。战士们极少请他们占卜，因为如果知道什么时候会死，就不可能去投身于一场战斗。战士们宁愿体验拼杀的滋味，体验生死未卜的激动。未来已由安拉写定，而无论安拉所写定的是什么，都总是为了有益于人类。所以战士们只为现在而活着，因为现在充满着各种意外，他们必须要关注许多事情:敌人的剑在何处，马在哪里，下一次应该出何种招术才能保全生命。 

赶驼人不是战士，他己请教过几位占卜师。他们中许多人的预言是正确的，另外一些人的预言则是错误的，直到有一天，他们中年纪最老(也最令人敬畏)的占卜师问赶驼人，为什么他对知道自己的未来如此感兴趣。 

"为了能有所行动，"赶驼人回答说，"改变我不喜欢发生的那些事情。" 

"那样一来，它们就不再是你的末来了。"老占卜师回答说。 

"我想预知未来，也许是为了对将要发生的事情做好准备。"? 

"假如是好事而你并不知道，那就将是一个意外的惊喜。" 

占卜师说道，"假如是坏事而你己经知道，你就会在它发生之前忍受折磨。" 

"我所以想预知未来，因为我是个人，"赶驼人对占卜师说道，"而人是靠着对未来的希望而活的。" 

占卜师沉默了一阵儿。他是个玩掷签的行家:把签掷在地上，然后根据它们落地的形状作出解释。那一天他没有掷签，而是把它们包进一块手帕，又放进了衣袋里。 

"他们并不关心预兆。他们相信，如果他们必须知道安拉想要告诉他们什么，就会有某个人来讲给他们听。这种事以前已发生过许多次。不过今天要讲给他们听的那个人就是你。" 


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
        url: '/pages/book3/mulu/12/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book3/muyangshaonian/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book3/mulu/14/main'
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
