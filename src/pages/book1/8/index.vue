<template>
  <div class="counter-warp">
                   <div text-align="center">第八章</div>
                   <div class="home">
   “噢——哥！噢——哥！”

孙玉厚老汉刚把自己的铺盖卷儿搬到隔壁少安的小土窑里，就听见公路下面他弟玉亭喊叫他的声音。

玉厚奇怪：玉亭为什么不上家里来？往常他有事没事吃完饭总要到他家里来坐一阵——穿着麻绳子捆绑的烂鞋，往他家前炕的铺盖卷上一靠，没命地在他的烟布袋里挖得抽半天烟。他热心公家的事，庄稼行里又不行，因此管务不起来旱烟，满年四季都是他供着。每当玉亭来的时候，他老婆也总要把家里刚吃过而剩下的饭，给玉亭热得端上来一碗。玉亭嘴里推让着，两只手一把就接住了。少安他妈知道玉亭在家里吃不饱，总要牵挂着给他吃一点。父亲去世早，玉亭从五岁起，实际上就是他两口子一手把他带大的。尽管玉亭成家以后，他老婆贺凤英那些年把少安妈欺负上一回又一回，怕老婆的玉亭连一声也不敢吭，但少安他妈不计较他。因为她从小把玉亭抚养大，心中对他有一种疼爱的感情。人常说，老嫂为母，这话可一点也不假……“噢——哥！噢——哥！”

玉亭仍然一声接一声地在公路下面喊叫。

玉厚听见他弟这样喊叫，又不上他家来，不知出了什么事，就一边从院子里往外走，一边给下面的玉亭答应了一声。在院子外的小土坡上往下走的时候，玉厚心里才恍然大悟：他弟弟今晚上不上他家来，是因为他女婿今天被“劳教”了。玉亭现在公社正看得起，让他当了会战指挥部的副总指挥。现在他家里出了“阶级敌人”，玉亭怕人家说他划不清界线，因而连累了他，所以才不上他家里来了。玉厚来到公路上，半天才看清他弟站在路边一棵树影下。他走过去，问：“什么事？”

“唉，也没什么事。想和你拉两句话……你心放宽些！”

玉亭脸上是一副同情他哥的神色。这同情是真诚的，因为这终究是他哥嘛！

玉厚没有说什么话，沉默地从自己的烟布袋里挖了一锅烟，点着抽起来。

玉亭也从身上掏出自己的烟锅，在他哥的烟布袋里挖了一锅，又用他哥的火柴点着，说：“满银一脑子的资本主义。劳教两天是小事，再不学习和改正，说不定要进班房。亲戚都要为这小子在政治上受影响……”

玉厚还是一声不吭。他现在已经懒得再说他女婿的长长短短。他心里只是为他的女儿和两个外孙难受。

今晚上公社要在学校开批判会，少安没回来，你家里其他人参加不成，你歪好要去一下，不要叫人家说，你们家抵制批判亲属的资本主义倾向……”玉亭对他哥说。“我不去！不劳动不行，不开会还不行！”

“哥，你不敢这样。咱们是贫下中农，毛主席号召的事，咱怎能不积极哩？”玉亭劝他哥说。

“反正我不参加！我的气已经受够了！哪怕明天让我也劳教哩！”

玉厚说完，气恼地转过身就往回去。他心里烦乱，有什么心思站在公路上讨论这号事情哩！

玉亭看他哥这样犟，也无可奈何了。要是村里其他人敢这样“反动”，他早就给会战总指挥部汇报了；恐怕今晚上也得上批判台。唉！玉亭心里烦透了，正在他被公社重用的时候，亲属中间突然出现这么一件叫他尴尬的事！

玉亭失望地见他哥快上了土坡，就又轻轻喊叫了一声：“哥，你先等一等……”



孙玉亭匆忙地从金俊山家的土坡上下来，顺着哭咽河畔的小路，向金家湾后面的小学赶去。他远远地看见，那里已经闪烁起灯火，并且聚集起一大片熙熙攘攘的人群……
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
        url: '/pages/book1/7/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book1/9/main'
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