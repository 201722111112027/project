<template>
  <div class="counter-warp">
     <div class="title" text-align="left">围城</div>
     <div text-align="center">前言</div>
     <div class="title" text-align="left">重印前记</div>
      
     <div class="home" >
     
　　<p>在这本书里，我想写现代中国某一部分社会、某一类人物。</p>写这类人，我没忘记他们是人类，只是人类，具有无毛两足动物的基本根性。角色当然是虚构的，但是有考据癖的人也当然不肯错过索隐的杨会、放弃附会的权利的。 
　　这本书整整写了两年。两年里忧世伤生，屡想中止。由于杨绛女士不断的督促，替我挡了许多事，省出时间来，得以锱铢积累地写完。照例这本书该献给她。不过，近来觉得献书也像“致身于国”、“还政于民”等等佳话，只是语言幻成的空花泡影，名说交付出去，其实只仿佛魔术家玩的飞刀，放手而并没有脱手。随你怎样把作品奉献给人，作品总是作者自已的。大不了一本书，还不值得这样精巧地不老实，因此罢了。 


　　　　　　　　　　　　　　　　三十五年【一九四九年】十二月十五日
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
        url: '/pages/book1/pfsj/main'
      })
    },
    list(){
      wx.navigateTo({
        url: '/pages/book1/pfsj/main'
      })
    },
    next(){
      wx.navigateTo({
        url: '/pages/book1/2/main'
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
