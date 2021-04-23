<template>
  <tab-bar>
    <tab-bar-item path="/home">
      <img eslint-plugin-vue="item-icon" src="~assets/img/tabbar/home.svg" alt="">
      <img eslint-plugin-vue="item-icon-active" src="~assets/img/tabbar/home_active.svg" alt="">
      <div eslint-plugin-vue="item-text">首页</div>
    </tab-bar-item>
  </tab-bar>
  <h2>shshhshss </h2>
</template>

<script>
  import TabBar from 'components/common/tabbar/TabBar'
import TabBarItem from '../../common/tabbar/TabBarItem.vue'

  export default {
    name: "MainTabbar",
    components: {
      TabBar,
      TabBarItem
    } 
  }
</script>

<style scoped>

</style>