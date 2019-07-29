<template>
  <div>
<div class="header">
	 <div class="top">
		 <router-link to='/mine'><img src="../../../static/img/i_back.png" alt=""></router-link>
		  <span>登录</span>
		  	<router-link to='/register'>注册</router-link>
	 </div>
</div>
<div class="beijing"></div>
<div class="form">
	<form action="">
		 <div class="one"><img src="../../../static/img/sign_icon_phone01.png" alt="" class="img"><input type="text" placeholder="用户名/手机号"></div>
		 <div class="tow"><img src="../../../static/img/sign_icon_lock01.png" alt="" class="img"><input type="text" placeholder="用户名/手机号"> <img src="../../../static/img/sign_icon_eye01.png" alt="" class="kan"></div>
     <button>登录</button>	
	</form>
	<a href="">忘记密码</a>
</div>
<div class="box">
	<div class="foot">
		<h2>第三方登录</h2>
		<div class="myfoot">
			 <div>
				  <img src="../../../static/img/weixin.png" alt="">
					<p>微信</p>
			 </div>
			   <div>
			 			  <img src="../../../static/img/qq.png" alt="">
			 				<p>QQ</p>
			   </div>
		</div>
	</div>
</div>
 

  </div>
</template>

<script>
  export default{

  }
</script>

<style lang="less" scoped>
	.header{
		width: 100%;
		height: 130/64rem;
		 border-bottom: 1px solid #000;
	}
.top{
	font-size: 32/64rem;
	display: flex;
	width: 580/64rem;
	height: 130/64rem;
	 margin: 0 auto;
	 line-height: 160/64rem;
	 font-weight: 600;
	 
	img{
		width: 20/64rem;
		height: 30/64rem;
	}
	span{
		flex: 1;
		text-align: center;
	}
	a{
		color:#6392ef;
	}
	}
	.beijing{
		width: 100%;
		height:40/64rem;
		background:#f2f2f2;
	}
	form{
		width: 100%;
		input{
			height:60/64rem;
			width: 460/64rem;
			 position: relative;
			 left:50/64rem;
			 top:10/64rem;
			 font-size: 27/64rem;
			 border: none;
		}
		.one{
			border: none;
		}
		div{
			background: #fff;
			 position: relative;
			 height: 110/64rem;
			 border: 1px solid #ccc;
			 
			 .img{
				 width:35/64rem;
				 height: 45/64rem;
				 position: relative;
         left:25/64rem;
				 top:25/64rem;
			 }
			 .kan{
				 position: absolute;
				 width:40/64rem;
				 height:26/64rem;
				 right: 30/64rem;
				 top:50/64rem;
			 }
		}
		button{
			width: 580/64rem;
			height: 92/64rem;
			color: #fff;
			font-size: 32/64rem;
			background:#5f8cf7;
			border-radius: 15/64rem;
			margin:45/64rem 30/64rem;
		}
	}
	.form a{
		font-size:32/64rem;
		color: #779cf5;
		 margin-left:475/64rem;
	}
	.form{
		height: 100%;
		background:#f2f2f2;
	}
	.box{
		height: 100%;
		width: 100%;
		background:#f2f2f2;
	}
	.foot{
		position: relative;
		top:200/64rem;
		height:200/64rem;
		height:250/64rem;
		background: #fff;
		.myfoot{
			
			width: 100%;
			display: flex;
			div{
				flex: 1;
				text-align: center;
				 position: relative;
				top:60/64rem;
				img{
					width: 87/64rem;
					height: 87/64rem;
				}
				p{
					font-size: 28/64rem;
				}
			}
		}
		h2{
			text-align: center;
			color: #999;
			 position: relative;
			 top:30/64rem;
			 
		}
	}
	 
</style>
