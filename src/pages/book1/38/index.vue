<template>
  <div class="counter-warp" >
                   <div text-align="center">第三十八章</div>
                   <div class="home">
  <p>孙少安其实并没有任何可办的事。</p>他只是感到一种无法言语的难受和痛苦，不愿意和父亲、妹妹一块相跟着回家。他想一个人度过一段时间，让积压在胸中的闷气慢慢消散出去。

他在人迹稀稀拉拉的石圪节街上毫无目的地遛达着。尽管一天只吃了一顿饭，也觉得不饥饿。好在街上再没碰见熟人，他可以把精神集中在自己的内心。


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