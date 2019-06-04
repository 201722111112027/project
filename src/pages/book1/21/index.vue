<template>
  <div class="counter-warp" >
                   <div text-align="center">第二十一章</div>
                   <div class="home">
  <p>实际上，田福堂在看见润叶和少安正晌午坐在河滩里的一刹那间，</p>心里就什么都清楚了。他又不是没年轻过嘛！那时虽然是旧社会，但这号事旧社会和新社会有什么区别？只不过他那时可不敢和润叶她妈大白天坐在河滩里罢了。

使他大吃一惊的是，他的润叶怎能看上了孙少安？

啊呀，这是他做梦也想不到的！虽说两个娃娃小时候一块耍大，但以后一个在农村受了苦，一个到城里上学，又参加了工作，现在等于说天上地下一般，两个人怎么能往这件事上想呢？再说，撇过孙少安不论，他们那家庭又是个什么样的烂滩场！他有文化有工作的女儿怎么可能嫁给他们呢？这不是全中国的一件怪事吗？

田福堂都由不得失笑了。

但是一认真想这事，他便感到又震惊又慌乱。哈呀，他没想到他女儿看起来腼腼腆腆，心胆倒挺大！哼，她凭什么能看上个孙少安？而且还敢在光天化日下坐在村外面谈恋爱哩！他现在才知道，润叶这几次回家来，慌慌乱乱，心神不定，动不动就跑出去了——原来她这都是为了孙玉厚那个大小子啊！

不行！他就是寻死上吊，也不会同意让他的女儿进了孙玉厚的家门！虽说现在兴男女婚姻自由，但不能自由得没框没架，没棱没沿嘛！别说是真的进了孙家的门，就是他的工作女儿和一个泥腿把子谈恋爱这件事，若是让村邻乡舍都知道，他田福堂的脸都没处搁。

他要很快制止这件丑事继续发展。当然，他是个精明人，也不愿伤自己娃娃的脸。因此自发生这件事后，一直装得和不知道一样……

女儿回县城已经三天了，现在田福堂的心情还平静不下来。这几天他已经没心思管村里的工作，日夜盘算润叶和少安的事。

他有时也豁达地想，如果少安当年不要回来劳动，和润叶一块去上学，再寻个工作，那这娃娃做他的女婿说不定还可以。少安本人他看上哩！要是文化再高一点，又有工作，说不定将来还能熬个大官……反过来再说，要是他女儿没文化没工作，也在双水村劳动，农民对农民，那不要他孙少安骚情，他田福堂会直接找媒人把润叶许配给他的。当然，如果是这样，他也就不会嫌孙玉厚家穷了，到时候他会把少安的光景扶起来的：没地方住吗？他给箍两孔新窑！没吃的吗？到他家里来吃！

可是，现在明摆着，两个人的条件差得太远嘛！

他想，孙少安这小子也不知道个天高地厚！你不在东拉河里照照你的影子，看能不能配上我润叶？你胡骚情我女儿，最后就是落了空，你除损失不了什么，还能抬高你的身价哩！可你等于给我田福堂祖坟供桌上撒了一泡尿！活活地往死欺负人哩！哼！你小子甭能！我田福堂也不是个省油的灯盏！



田福堂若有所思地站了一会，然后说他去买个东西，就和田福高打了个招呼，调转车子过了桥，向石圪节的街上走去……
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
        url: '/pages/book1/20/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book1/22/main'
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