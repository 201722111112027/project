<template>
  <div class="counter-warp" >
                   <div text-align="center">第十七章</div>
                   <div class="home">

  <p>开学已经两个多星期，孙少平还没有机会和郝红梅单独说话。</p>

他看见红梅换了一件半旧的红格子布衫，好象变了另外一个人似的。大概由于一个假期在家里，这个季节吃的东西又比较多一些，她原来很瘦削的脸颊现在看起来丰满了许多。已经度过了半年的城市生活，她也懂得把自己农村式的“家娃”头，象城市姑娘一样扎起了两个短辫；加上自做的、手工精细的方口鞋和一条看起来是新买的天蓝色裤子，简直让人都认不出来这就是郝红梅了。其实她无非就是把原来的一身补钉衣服换成了没有补钉的衣服。这个小小的变化，就使一个本来不显眼的人，一下子很引人注目了。同时也应该承认，郝红梅本来就具备那种漂亮姑娘的脸型和身段。如果有一身比现在更漂亮的衣服，就很难看出这姑娘是来自农村了。

孙少平看见她，心中就会荡起一股热辣辣的激流，有时甚至感到呼吸都有了困难。

当然，他自己的衣服还是老模样。一身家织的老粗布，尽管金波妈给他裁剪成制服式样，但仍然不能掩饰它本质上的土气；加上暑假给家里砍柴，被活柴活草染得肮肮脏脏，开学前快把家里蒸馍的半碗碱面用光了，还是没有洗净。他看着这身叫他伤心的衣服，真想一把脱了扔掉。可自己很快又苦笑了：扔掉只得光身子跑！唉，最使他脸红的是，他这么大了，连个裤衩都做不起。晚上睡觉，人家都脱了长衣服穿着裤衩，他把外衣一脱就赤条条一丝不挂了……但不论怎么说，他现在有一个甜蜜的安慰：就他这副穷酸样，班里也许是最俊的女子还和他相好哩！让侯玉英见鬼去吧！她就是想和他好，他也不愿意呢！这倒不是嫌她的腿——假如红梅的腿是跛的，他也会和她相好的！

可是眼看半个多月过去了，少平还是没能和红梅拉几句话。这倒不是说连一点机会也没。其实他们单独碰见过好多次，但不知她为什么又象上学期那样躲开了——而且常常看来是有意回避他！

少平对此摸不着头脑。想来想去，他连一点原因也找不出来。

不过，他现在还没忙着象上学期一样陷入苦恼之中。他猜想：也许红梅家里有什么事，她心里烦乱，才不愿意和他说话。

但看来她又没什么烦乱！相反，她却比上学期活跃多了。现在甚至每天下午吃完饭，在男女混杂的篮球场上，都能看见她说说笑笑和同学们一块玩呢！

于是，有一天下午，少平看见红梅又在篮球场上的时候，他自己也就旋磨着进了场。这并不是比赛，两边篮板下都有许多男女同学，站成一个半圆，谁捉住球，谁投篮。不管谁，投了一次篮紧接着又拿到球的时候，就传给另外一个人——他们都是高中生了，已经懂得规矩和礼貌。

少平看见红梅投了一次篮后，球又一次回到她手里。看她准备给别人传时，少平就在她后边说：“给我一个！”

红梅不会没有听见他说话，但她没有理他，甚至连头也没有回，把球传给了另外一边的班长顾养民。

本来少平已经伸出了手，但却又不得不尴尬地把手缩回来。刹那间，他感到浑身的血都向脸上涌来，眼睛也好象蒙上了一层灰雾，远远近近什么也看不清楚了。


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
        url: '/pages/book1/16/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book1/18/main'
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