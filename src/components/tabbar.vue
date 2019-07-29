<template>
  <div class="tabbar">
    <item-wrap title='首页' mark='home' :curr='currindex' @change='changValue' class='childbar'>
      <img class="imgTop" src="../../static/img/i_main_home.png" alt="" slot='imgTop'>
      <img class="imgTop" src="../../static/img/i_main_home_activity.png" alt="" slot='imgbottom'>
    </item-wrap>
    <item-wrap title='问答' mark='question' :curr='currindex' @change='changValue' class='childbar'>
      <img class="imgTop" src="../../static/img/i_main_qa.png" alt="" slot='imgTop'>
      <img class="imgTop" src="../../static/img/i_main_qa_activity.png" alt="" slot='imgbottom'>
    </item-wrap>
    <item-wrap title='班级' mark='className' :curr='currindex' @change='changValue' class='childbar'>
      <img class="imgTop" src="../../static/img/i_main_study.png" alt="" slot='imgTop'>
      <img class="imgTop" src="../../static/img/i_main_class_activity.png" alt="" slot='imgbottom'>
    </item-wrap>
    <item-wrap title='我的' mark='mine' :curr='currindex' @change='changValue' class='childbar'>
      <img class="imgTop" src="../../static/img/i_main_mine.png" alt="" slot='imgTop'>
      <img class="imgTop" src="../../static/img/i_main_mine_activity.png" alt="" slot='imgbottom'>
    </item-wrap>
  </div>
</template>

<script>
  import itemWrap from './itemWrap.vue'

  export default {
    data: function() {
      return {
        currindex: 'home',
      }
    },
    components: {
      itemWrap,
    },
    methods: {
      changValue(value) {
        this.currindex = value;
      }
    },
    mounted() {
      this.$router.push({
        path: '/home/recommended'
      })
    }

  }
</script>

<style scoped lang="less">
  .tabbar {
    background-color: white;
    display: flex;
    justify-items: center;
    align-items: center;
    text-align: center;
    position: fixed;
    bottom: 0;
    width: 100%;
    height: 105/75rem;


  }

  .childbar {

    flex: 1;

    .imgTop {
      width: 40/75rem;
      height: 40/75rem;
    }
  }
</style>
