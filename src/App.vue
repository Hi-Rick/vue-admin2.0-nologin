<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
  html, body{
    width: 100%;
    height: 100%;
    margin: 0;
    padding: 0;
    background-color: #f2f2f2;
  }
  .el-scrollbar__wrap{
    overflow-x: hidden;
  }
</style>
