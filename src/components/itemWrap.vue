<template>
  <div @click="fn">
    <span v-show='!flag'>
      <slot class='imgTop' name="imgTop"></slot>
    </span>

    <span v-show='flag'>
      <slot class='imgTop' name="imgbottom"></slot>
    </span>
    <p :class="{title:flag}">{{title}}</p>
  </div>
</template>

<script>
  export default {

    data() {
      return {
        showImg: false,
      }
    },
    props: ['title', 'curr', 'mark'],
    computed: {
      flag() {
        if (this.mark == this.curr) {
          return true;
        }
        return false;
      }
    },
    methods: {
      fn() {
        this.$emit('change', this.mark)
        this.$router.push({path:'/'+this.mark})
      }
    }
  }
</script>

<style scoped lang="less">
  .title {
    color: #69a5db;
  }
</style>
