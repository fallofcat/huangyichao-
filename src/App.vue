<template>
  <div>

    <router-view />
    <tabbar></tabbar>
  </div>
</template>

<script>
  import tabbar from './components/tabbar.vue'
  export default {
      components:{
        tabbar
      }
  }
</script>

<style>
  * {
    padding: 0;
    margin: 0;
    text-decoration: none;
    list-style: none;
  }
</style>
