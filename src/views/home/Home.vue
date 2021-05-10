
<template>
  <div id='home'>首页</div>  
<nav-bar>
  <template v-slot:center>
  
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