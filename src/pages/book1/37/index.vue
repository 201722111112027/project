<template>
  <div class="counter-warp" >
                   <div text-align="center">第三十七章</div>
                   <div class="home">
  <p>孙少安其实并没有任何可办的事。</p>他只是感到一种无法言语的难受和痛苦，不愿意和父亲、妹妹一块相跟着回家。他想一个人度过一段时间，让积压在胸中的闷气慢慢消散出去。

他在人迹稀稀拉拉的石圪节街上毫无目的地遛达着。尽管一天只吃了一顿饭，也觉得不饥饿。好在街上再没碰见熟人，他可以把精神集中在自己的内心。

直等到太阳落山以后，他才一个人慢慢地通过石圪节那座小桥，踏上了通往双水村的公路。

走不多远，天色已经完全暗下来了。不过，快要满圆的月亮从东拉河对面的山背后静悄悄地露出脸来，把清淡的光辉洒在山川大地上。万物顿时又重新显出了面目，但都象盖了一层轻纱似的朦朦胧胧。暑气消散，大地顿时凉爽下来。公路两边庄稼地里的无名小虫和东拉河里的蛤蟆叫声交织在一起，使这盛夏的夜晚充满了纷扰和骚乱。

孙少安穿一件破烂的粗布小褂，外衣搭在肩头，吸着自卷的旱烟卷，独个儿在公路上往回走。他有时低倾着头；有时又把头扬起来，猛地站住，茫然地望着迷乱的星空和模糊的山峦。一声长叹以后，又迈开两条壮实的长腿走向前去……痛苦，烦恼，迷茫，他的内心象洪水一般泛滥。一切都太苦了，太沉重了，他简直不能再承受生活如此的重压。他从孩子的时候就成了大人。他今年才二十三岁，但他感觉到他已经度过了人生的大部分时间。没吃过几顿好饭，没穿过一件象样的衣服，没度过一天快活的日子，更不能象别人一样甜蜜地接受女人的抚爱……什么时候才能过几天轻松日子？人啊！有时候都比不上飞禽走兽，自由自在地在天空飞，在地上走……

一种委屈的情绪使他忍不住泪水盈眶。他停在路边的一棵白杨树下，把烫热的脸颊贴在冰凉的树干上，两只粗糙的手抚摸着光滑的杨树皮，透过朦胧的泪眼惆怅地望着黑糊糊的远山。公路下面，东拉河的细流发出耳语似的声响。夏夜凉爽的风从川道里吹过来，摇曳着树梢和庄稼。月亮升高了，在清朗的夜空冷淡地微笑着。星星越来越繁密，象在一块巨大的青石板上缀满了银钉……孙少安在白杨树下站了一会，又开始往回走。走不多远，他就看见了双水村星星点点的灯火。

一股温暖的激流刹那间漫过了他的心间。那灯光下，有他亲爱的家——亲人们的脸庞都在他的眼前浮现出来了。

于是，头脑中迷茫的云雾顷刻间消散，滚烫的额头重新又凉了下来。他顿时感到他刚才的情绪充满了危险。是的！一家老老少少都依靠和指望着他，他怎么能这样胡思乱想呢？不，他应该象往常一样，精神抖擞地跳上这辆生活的马车，坐在驾辕的位置上，绷紧全身的肌肉和神经，吆喝着，呐喊着，继续走向前去。如果他垮了，说不定人仰马翻，一切都完了……

他弯下腰在路边拾起一块石头，抡起胳膊，狠狠地甩向了东拉河对面的山洼上，好象要把他的一切烦恼都随着这块石头抛出去。

他匆匆把外衣穿上，也没扣钮扣，就向村子里走去。

临进村子时，他为了使自己的心情平静下来，想在什么地方坐一坐。公路边不合适，万一村里有人看见他黑天半夜坐在野地里，会乱猜测的。

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