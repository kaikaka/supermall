<template>
    <div class="tab-bar-item" @click="itemClick">
      <div class="icon-img" v-if="!isActive"><slot name="item-icon"></slot></div>
      <div v-else><slot name="item-icon-active"></slot></div>
      <div :style="activeStyle"><slot name="item-text"></slot></div>
    </div>  
</template>

<script>
export default {
  name: "TabBarItem",
  props: {
    path: {
      type: String,
      default: './home'
    },
    activeColor: {
      type: String,
      default: 'red'
    }
  },
  data() {
    return {}
  },
  computed: {
    isActive() {
      return this.$router.currentRoute.value.path === this.path
    },
    activeStyle() {
      return this.isActive ? {color:this.activeColor} : {}
    }
  },
  methods: {
    itemClick() {
      this.$router.replace(this.path)
    }
  }
}
</script>

<style scoped>
  .tab-bar-item {
    flex: 1;
    text-align: center;
    height: 49px;
    font-size: 14;
  }

  .icon-img {
    display: block;
    height: 24px;
    margin-top: 3px;
    margin-bottom: 2px;
    text-align: center;
  }

</style>