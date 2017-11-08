<template>
  <div class="hello">
    <el-row>
      <el-col :span="12"><div class="grid-content bg-purple">teste1</div></el-col>
      <el-col :span="12"><div class="grid-content bg-purple-light">teste 2</div></el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
