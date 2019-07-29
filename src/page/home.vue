<template>
  <div>
    <homehead>
      <img src="../../static/img/ic_home_title_left.png" alt="" class='imgleft img' slot='imgleft'>
      <img src="../../static/img/ic_home_title_right.png" alt="" class='imgright img' slot='imgright'>
    </homehead>




    <router-view></router-view>
  </div>
</template>

<script>
  import homehead from '../components/home/homeHead.vue'
  export default {
    components: {
      homehead
    },

  }
</script>

<style scoped lang="less">

</style>
