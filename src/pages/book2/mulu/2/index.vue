<template>
  <div class="counter-warp">
     <div class="title" text-align="left">围城</div>
     <div text-align="center">第二章</div>

      
     <div class="home" >
     
　　<p>据说“女朋友”就是“情人”的学名，说起来庄严些，正像玫瑰在生物学上叫“蔷薇科木本复叶植物”，</p>或者休妻的法律术语是“协议离婚”。方鸿渐陪苏小姐在香港玩了两天，才明白女朋友跟情人事实上绝然不同。苏小姐是最理想的女朋友，有头脑，有身分，态度相貌算得上大家闺秀，和她同上饭馆戏院并不失自己的面子。他们俩虽然十分亲密，方鸿渐自信对她的情谊到此而止，好比两条平行的直线，无论彼此距离怎么近，拉得怎么长，终合不拢来成为一体。只有九龙上岸前看她害羞脸红的一刹那，心忽然软得没力量跳跃，以后便没有这个感觉。他发现苏小姐有不少小孩子脾气，她会顽皮，会娇痴，这是仇一向没想到的。
　　可是不知怎样，他老觉得这种小妞儿腔跟苏小姐不顶配。并非因为她年龄大了；她比鲍小姐大不了多少，并且当着心爱的男人，每个女人都有返老还童的绝技。
　　只能说是品格上的不相宜；譬如小猫打圈儿追自己的尾巴，我们看着好玩儿，而小狗也追寻过去地回头跟着那短尾巴橛乱转，说风趣减少了。那几个一路同船的学生看小方才去了鲍小姐，早换上苏小姐，对他打趣个不亦乐乎。
　　苏小姐做人极大方；船到上海前那五六天里，一个字没提到鲍小姐。她待人接物也温和了许多。方鸿渐并未向她谈情说爱，除掉上船下船走跳板时扶她一把，也没拉过她手。可是苏小姐偶然的举动，好像和他有比求婚、订婚、新婚更深远悠久的关系。她的平淡，更使鸿渐疑惧，觉得这是爱情热烈的安稳，仿佛飓风后的海洋波平浪静，而底下随时潜伏着汹涌翻腾的力量。香港开船以后，他和苏小姐同在甲板上吃香港买的水果。他吃水蜜桃，耐心地撕皮，还说：“桃子为什么不生得像香蕉，剥皮多容易！或者干脆像苹果，用手帕擦一擦，就能连皮吃。”苏小姐剥几个鲜荔枝吃了，不再吃什么，愿意替他剥桃子，他无论如何不答应。桃子吃完，他两脸两手都持了幌子，苏小姐看着他笑。他怕桃子汁弄脏裤子，只伸小指头到袋里去勾手帕，勾了两次，好容易拉出来，正在擦手，苏小姐声音含着惊怕嫌恶道：“啊哟！你的手帕怎么那么脏！真亏你——哙！这东西擦不得嘴，拿我的去拿去，别推，我最不喜欢推。”
　　
　　丈母道：“鸿渐这样老实，是找不到女人的。让我为他留心做个媒罢。”
　　丈人道：“你又来了！他老太爷、老太太怕不会作主。咱们管不着。”
　　丈母道：“鸿渐出洋花的是咱们的钱，他娶媳妇，当然不能撇开咱们周家。
　　
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
        url: '/pages/book2/mulu/1/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book2/weicheng/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book2/mulu/3/main'
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
