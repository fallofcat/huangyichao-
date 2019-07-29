<template>
  <div class="content">
    <div class="container">
      <mt-swipe :auto='2000'>
        <mt-swipe-item>
          <img class="autoImg" src="../../../static/img/banner.jpg" alt="">
        </mt-swipe-item>
        <mt-swipe-item>
          <img class="autoImg" src="../../../static/img/banner1.jpg" alt="">
        </mt-swipe-item>
        <mt-swipe-item>
          <img class="autoImg" src="../../../static/img/banner2.jpg" alt="">
        </mt-swipe-item>
        <mt-swipe-item>
          <img class="autoImg" src="../../../static/img/banner3.jpg" alt="">
        </mt-swipe-item>
      </mt-swipe>
    </div>
    <div class="livebroadcastClass">
      <div class="livebroadcastClass-title">
        <h4>直播公开课</h4>
        <p>更多<img src="../../../static/img/image/rectangle.png" alt=""></p>
      </div>
      <div class="livebroadcastClass-content">
        <mt-swipe :auto="0">
          <mt-swipe-item v-for="item in livebroadcastClassData">
            <p>item.class</p>


          </mt-swipe-item>
          <mt-swipe-item>2</mt-swipe-item>
          <mt-swipe-item>3</mt-swipe-item>
        </mt-swipe>
      </div>
    </div>



  </div>
</template>
<script>
  // import 'mint-ui/lib/style.css'
  export default {


    data:function (){
      return{
        livebroadcastClassData:[],
      }
    },
    mounted() {
      this.$axios.get("../../../static/data/recommededData/recommededData.json")
      .then(function(shuju){
          console.log(shuju.data);
          this.livebroadcastClassData=shuju.data
      })
    }
  }
</script>
<style lang="less" scoped>
  .content {
    margin: 0 30/75rem;
  }

  .container {
    position: relative;
    left: 50%;
    transform: translateX(-50%);
    border-radius: 15/75rem;
    width: 696/75rem;
    height: 194/75rem;

    .autoImg {
      border-radius: 15/75rem;
      width: 100%;
      height: 100%;
    }
  }

  .livebroadcastClass {
    .livebroadcastClass-title {
      padding: 50/75rem 0 28/75rem 0;
      display: flex;
      line-height: 30/75rem;
      align-items: center;
      position: relative;

      h4 {
        font-size: 28/75rem;
      }

      p {
        display: flex;
        align-items: center;
        position: absolute;

        right: -10/75rem;

        img {
          width: 30/75rem;
        }
      }
    }

    .livebroadcastClass-content {
      width: 696/75rem;
      height: 232/75rem;
      border-radius: 15/75rem;
      box-shadow: 4px 5px 10px #ccc;
    }
  }
</style>
