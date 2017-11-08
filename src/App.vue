<template>
  <div id="app">
    <header-app></header-app>
    <router-view></router-view>
  </div>
</template>

<script>
import Header from '@/components/Layout/Header'

export default {
  name: 'app',
  components: {
    'header-app': Header
  }
}
</script>

<style>
.el-menu-demo {
  margin-bottom: 60px;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
