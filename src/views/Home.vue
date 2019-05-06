<template>
  <div class="main-box">
    <h2 class="main-title">JS组件</h2>
    <ul class="main-list">
      <li v-for="(item, index) in jsCompts" :key="index">
        <span class="indexicon" :class="item.icon"></span>
        <p>{{item.name}}</p>
        <i class="icons-chevron-right"></i>
      </li>
    </ul>
    <h2 class="main-title">JS组件</h2>
  </div>
</template>

<script>

// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {

  },
  data: function() {
    return {
      jsCompts: [{
        name: '提示框',
        icon: 'icon-toast',
        herf: ''
      },{
        name: '指示符',
        icon: 'icon-indicator',
        herf: ''
      },{
        name: '拉下',
        icon: 'icon-pull-down',
        herf: ''
      },{
        name: '拉起',
        icon: 'icon-pull-up',
        herf: ''
      },{
        name: '无限滚动',
        icon: 'icon-infinite-scroll',
        herf: ''
      },{
        name: '消息框',
        icon: 'icon-message-box',
        herf: ''
      },{
        name: '行动表',
        icon: 'icon-action-sheet',
        herf: ''
      },{
        name: '弹出',
        icon: 'icon-popup',
        herf: ''
      },{
        name: '刷卡',
        icon: 'icon-swipe',
        herf: ''
      },{
        name: '懒加载',
        icon: 'icon-lazyload',
        herf: ''
      },{
        name: '范围',
        icon: 'icon-range',
        herf: ''
      },{
        name: '进展',
        icon: 'icon-progress',
        herf: ''
      },{
        name: '选择器',
        icon: 'icon-picker',
        herf: ''
      },{
        name: '日期时间选择器',
        icon: 'icon-time',
        herf: ''
      },{
        name: '索引列表',
        icon: 'icon-alphabet',
        herf: ''
      },{
        name: '调色板按钮',
        icon: 'icon-alphabet',
        herf: ''
      }]
    }
  }
}
</script>

<style lang="less" scoped>
.main-title{
  line-height: 1.4rem;
  padding: 1rem 0;
  text-align: center;
  font-size: 1.4rem;
}
.main-list{
  background: #fff;
  overflow: hidden;
  li {
    position: relative;
    padding: 0 0 0 2.5rem;
    overflow: hidden;
    span {
      position: absolute;
      top: 50%;
      left: 0.5rem;
      width: 1.4rem;
      height: 1.4rem;
      line-height: 1.4rem;
      margin: -0.6rem 0 0;
      color: #26a2ff;
    }
    i {
      position: absolute;
      top: 50%;
      right: 0.5rem;
      width: 1.4rem;
      height: 1.4rem;
      line-height: 1.4rem;
      margin: -0.6rem 0 0;
      color: #999;
    }
    p {
      height: 2.8rem;
      line-height: 2.8rem;
      border-bottom: 0.0625rem solid #eee;
    }
  }
}

</style>
