<template>
<nav-bar class='home-nav'>
  <template v-slot:center>
  <div id='home'>首页</div>  
  </template>
</nav-bar>
</template>

<script>
import NavBar from '../../components/common/navbar/NavBar.vue'

  export default {
    name:"Home",
    components: {
        NavBar
    }
  }
</script>

<style>
.home-nav {
  background-color: var(--color-tint);
  color: white;
}

</style>