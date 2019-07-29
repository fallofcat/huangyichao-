<template>
  <div>
<mine>
      <img src="../../static/img/pen.png" alt="" class='imgleft img' slot='imgleft'>
      <img src="../../static/img/avatar_default.png" alt="" class='imgright img' slot='imgright'>
</mine>
  </div>
</template>

<script>
import mine from '../components/my/mine.vue'
  export default{
 components: {
      mine
   },
  }
</script>

<style lang="less">

	.imgright{
		width: 155/64rem;
   	height: 155/64rem;
   	position: absolute;
 	  right: 35/64rem;
	   top: 90/64rem;
	}
	.imgleft{
			width: 25/64rem;
 	   height: 25/64rem;
	}
</style>
