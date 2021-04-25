<template>
<div id="app"></div>
<router-view/>
<main-tab-bar/>
</template>

<script>
import MainTabBar from "./components/content/mainTabbar/MainTabBar"
import TabBar from './components/common/tabbar/TabBar.vue'
import TabBarItem from './components/common/tabbar/TabBarItem.vue'

export default {
  name: 'app',
  components: { TabBar ,MainTabBar, TabBarItem}
}
</script>

<style>
  @import "assets/css/base.css"
</style>
