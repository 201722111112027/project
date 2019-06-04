<template>
  <div class="counter-warp" >
                   <div text-align="center">第十八章</div>
                   <div class="home">
  <p>孙少平站在黄昏中的河岸边，思绪象乱麻一般纷扰。他明白，</p>从今往后，郝红梅再不可能和他相好了。他精神上最重要的一根支柱已经被抽掉，使他感到一种说不出来的痛苦。他面对着远方模糊的山峦，真想狂喊一声——他并不知道自己此刻眼里含满了泪水……在他背后，县城已经一片灯火灿烂了。家家户户现在也许都围坐在一起，开始吃晚饭。此刻，谁能知道，在城外，在昏暗的河边上，站着一个痛苦而绝望的乡下来的青年，他喉咙里堵塞着哽咽，情绪象狂乱的哈姆雷特一样……原谅他吧！想想我们在十七、八岁的时候，也许都有过类似他这样的经历。这是人生的一个火山活跃期，熔岩突奔，炽流横溢，在每一个感情的缝隙中，随时都可能咝咝地冒烟和喷火！

少平站在河边，尽管已经误了吃饭时间，但他一点也不感觉到饿。他突然幻想：未来的某一天，他已经成了一个人物，或者是教授，或者是作家，要么是工程师，穿着体面的制服和黑皮鞋，戴着眼镜，从外面的一个大地方回到了这座城市，人们都在尊敬亲热地和他打招呼，他在人群里看见了顾养民和郝红梅……

幻觉消失了，他看见一个黑乎乎的人影正向这边走来——他认出这是他的好朋友金波。

金波现在来到了他跟前。他把手里的四个玉米面烧饼递到他面前，说：“看你没回来，你的下午饭我吃了。这是我在街上给你买的……”

少平没有言传，接过金波手中的烧饼，坐在一块石头上吃起来。

金波也沉默不语地坐在他旁边。过了一会，他才咬牙切齿地说：“我想把顾养民捶一捶！”

金波显然看出顾养民已经夺走了他好朋友的女朋友，这使他胸膛里充满了义愤的怒火，想为少平打抱不平。

“打了他，说不定学校会把咱们开除了……”少平说。“你不要动手。由我出面！”

少平想了一下，说：“不敢这样。万一咱们出个事，能把家里的大人急死！”

“咱们现在就是大人了！自己做事自己可以承担。你不要管，我知道这事该怎么办哩！”

“你可千万不敢动手。咱们没什么理由打顾养民。要是平白无故打了，到时咱们没个说法的……”

“我给他制造个挨打理由！”

“不敢闯这乱子！”少平虽然和金波同岁，此刻心中又火烧火燎，但还是比他的朋友冷静一些。

金波也没再说话。等他把那四个玉米面饼吃完，他们就相跟着回学校去了。

孙少平没有想到，他的朋友没有听从他的劝告，在私下里开始积极筹划准备打顾养民了。



孙少平大开了一回眼界，然后带着无数新的印象以及一张奖状和一套“毛选”，回到了县城。到星期六的时候，他又带着从黄原城里买来的一点稀罕东西，回了一趟双水村。在地区期间，每天的伙食补助就够他吃了，因此他就把哥哥给他的十元钱，除过王满银，给全家人都买了点礼物：奶奶的一包蛋糕，母亲和姐姐一人一双袜子，父亲和哥哥一人一块白毛巾，妹妹的一线红方格头巾，猫蛋和狗蛋的半斤水果糖……
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
        url: '/pages/book1/17/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book1/19/main'
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