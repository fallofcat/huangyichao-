<template>
	<div>
		<div class="header">
			 <div class="top">
				 <router-link to='/login'><img src="../../../static/img/i_back.png" alt=""></router-link>
				  <span>注册</span>
			 </div>
		</div>
		<div class="beijing"></div>
		<div class="form">
			<form action="">
				 <div class="one"><img src="../../../static/img/sign_icon_phone01.png" alt="" class="img"><input type="text" placeholder="请输入注册手机号"><span class="myspan">验证码</span> </div>
				 <div class="tow"><img src="../../../static/img/safe42.png" alt="" class="img"><input type="text" placeholder="请输入验证码"></div>
				 <div class="tow"><img src="../../../static/img/sign_icon_lock01.png" alt="" class="img"><input type="text" placeholder="设置6位以上的密码"></div>
		     <button>下一步</button>	
			</form>
			 <div class="text">
				 <span>请按上面的“下一步”按钮，即表示你同意</span><br/>
				 <a href="">《网站用户注册及服务协议》</a>
			 </div>
		</div>
		 
		 
	</div>
</template>

<script>
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
				width: 400/64rem;
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
				 .myspan{
					 display: inline-block;
					 position: absolute;
					 top:20/64rem;
					 right: 10/64rem;
					 font-size: 25/64rem;
					 width: 130/64rem;
					 height: 60/64rem;
					 text-align: center;
					 line-height: 60/64rem;
					 background:#5f8cf7;
					 border-radius:8/64rem;
					 color: #fff;
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
		.text{
			margin-bottom:280/64rem;
			width: 100%;
			 text-align: center;
			 a{
				font-size:32/64rem;
				color: #779cf5;
			}
			 span{
				font-size:27/64rem;
				color:#999;
			}
		}
		 
		.form{
			height: 100%;
			background:#f2f2f2;
			 
			 
		}
		 
		 
</style>
