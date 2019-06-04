<template>
  <div class="counter-warp" >
                   <div text-align="center">第十二章</div>
                   <div class="home">

  <p>田润叶把中午饭从灶上打回来，放在炕头那个土台子炉灶上，</p>先没顾上吃。她端起一盆热水开始洗脸。

这一天够忙的了！早上，学校安排全校红小兵到城外去学军，而且统一规定学生都要穿黄衣服，男学生拿小马刀，女学生拿红缨枪。她是三年级的班主任，忙着检查学生们的这些“武器”是否齐备，服装是否符合学校要求。接着就带着孩子们在城外走了十几里路，捉了一会“特务”。回来累得睡了一阵，还没来得及洗脸，又是教师的集体政治学习时间，只好跑到会议室听学校革委会主任念了一篇“毛选”。眼下就是这样，一星期不上几天课，大都是教师带着学生，学军，种地，上街搞宣传，把人忙乱得不可开交。

她洗完脸，细心地梳理完头发，才搬了个小凳坐在炉灶前。她望着一碗土豆菜和一个玉米面馍怔怔地出神，还是没有动筷子。学校灶一个月只有二两细和六斤细粮，其余的都是玉米面和高粱米，菜总是白水煮土豆，里面没有几滴油。她忙了，就不回二爸家去，在学校凑合着吃这伙食。

润叶没动筷子，倒不是嫌这饭菜不好——尽管家庭条件优裕，但她从来不是个娇气人。她现在坐在这里发愣，是在想她的心事。

自从去年秋天以来，她二爸家出现了一个不速之客。起先她认不出来这个敦敦实实的青年是谁，但觉得有点面熟。后来她才知道，这是李叔叔家的儿子李向前。向前在中学时比她高两个年级，因此她并不熟悉这个人，当时见了面也只能大约判断象是一个学校的。

向前的父亲也是县革委会的副主任，和她二爸一块共事，到二爸家里来过好些次，她倒认识。向前的母亲听说是县医院的书记，是她二妈的领导，有时也来二妈家串门，她也认识。只是李向前以前从不上她二爸家来。

可是，自从去年秋天以来，他隔几天就来一回。每次来的时候，总要到她窑里来东拉西扯说半天话。他是县贸易经理部的汽车司机，经常跑外面，因此知道许多省城和外省的事，给她说个没完。每次临走时，他都问她在外地捎得买什么东西不？她都说不买。她在心里对这个人已经有点烦。她已听够了他那些沟里上洼里下的不上串话。但她不好意思表示她的反感——他父母亲和她二爸二妈一块共事，而且他妈还是她二妈的领导！

可是，有一天，他来的时候，竟然当着她二妈的面，拿出在省城买来的一件红线衣，对她说：“我碰上这么件衣服，觉得你穿上肯定合适，就给你捎着买来了。这是上海新出的一种线衣。哈呀，你不知道，买的时候，众人都抢，我插了一回队，还和一个人吵了一架，好不容易才买到了手……”

她有点生气了，说：“我不喜欢穿红颜色的衣服！”李向前手里举着那件来之不易的红线衣，感到十分尴尬。她二妈赶紧圆场说：“啊呀，你这娃娃！人家向前好心买了这衣服，你应该谢谢人家！再说，你怎不爱穿红颜色？你的毛衣不就是红颜色的吗？”

她的脸也成红颜色了。为了不让二妈难堪，她只好问向前：“多少钱？”

“钱什么哩……”向前吞吞吐吐地说。

“你受了这么大的麻烦，怎能连钱也不要哩！”她心里感到很不舒服。

“五……就五元钱！”向前只好说。

“不会是个整数吧？”

“零头我忘了……”

“你再想一想！”

“五元……噢，五元四角六……”


她只好把自己的门一锁，跟晓霞回她二妈家去了。
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
        url: '/pages/book1/11/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book1/13/main'
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