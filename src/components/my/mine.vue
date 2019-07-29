<template>
  <div class="mine">
 <div class="login">
					   <div class="mylogin">
								 <p><router-link to='/login' >登录/注册</router-link></p>
								  <p class="color"><slot name='imgleft'></slot><router-link to='/login'>成就更好未来</router-link></p>
						 </div>
					<router-link to='/login'><slot name='imgright'></slot></router-link>
				</div>
				 
				<div class="topbar">
					<div class="item">
					 <router-link to='/login'><img src="../../../static/img/ic_my_class.png" alt=""></router-link>
					 <p><router-link to='/login'>班级</router-link></p>
					</div>
					<div class="item">
						<router-link to='/login'><img src="../../../static/img/ic_my_download.png" alt=""></router-link>
						<p><router-link to='/login'>离线</router-link></p>
					</div>
					<div class="item">
						<router-link to='/login'><img src="../../../static/img/ic_my_msg.png" alt=""></router-link>
						<p><router-link to='/login'>消息</router-link></p>
					</div>
					<div class="item">
						<router-link to='/login'><img src="../../../static/img/ic_my_wechat.png"alt=""></router-link>
						<p><router-link to='/login'>微信</router-link></p> 
					</div>
				</div>
				<div class="bg"></div>
				<div class="content">
				<ul>
					<li>
						<router-link to='/login'>
							<img src="../../../static/img/ic_my_studycard.png" alt="" class="imgleft">
						  <span>学习卡</span>
							<img src="../../../static/img/i_more.png" alt="" class="imgright">
						</router-link>
					</li>
					<li>
						<router-link to='/login'>
							<img src="../../../static/img/ic_my_live.png" alt="" class="imgleft">
						  <span>我的公开课</span>
							<img src="../../../static/img/i_more.png" alt="" class="imgright">
						</router-link>
					</li>
					<li>
						<router-link to='/login'>
							<img src="../../../static/img/ic_my_qa.png" alt="" class="imgleft">
						  <span>我的问答</span>
							<img src="../../../static/img/i_more.png" alt="" class="imgright">
						</router-link>
					</li>
					<li>
						<router-link to='/login'>
							<img src="../../../static/img/ic_my_order.png" alt="" class="imgleft">
						  <span>我的订单</span>
							<img src="../../../static/img/i_more.png" alt="" class="imgright">
						</router-link>
					</li>
					<li>
						<router-link to='/login'>
							<img src="../../../static/img/ic_my_history.png" alt="" class="imgleft">
						  <span>浏览历史</span>
							<img src="../../../static/img/i_more.png" alt="" class="imgright">
						</router-link>
					</li>
					<li>
						<router-link to='/system'>
							<img src="../../../static/img/ic_my_setting.png" alt="" class="imgleft">
						  <span>系统设置</span>
							<img src="../../../static/img/i_more.png" alt="" class="imgright">
						</router-link>
					</li>
				</ul>
			</div>
  </div>
</template>

<script>
  export default{
 
  }
</script>

<style lang="less">
*{
margin: 0;
padding: 0;
}
.login{
	position: relative;
}
.mylogin {
	position: relative;
	top: 130/64rem;
	left: 37/64rem
}
.login a{
	color: #000;
	font-size:28/64rem;
}
.login p{
	margin-bottom: 15/64rem;
}
.login .color a{
	color:#666;
}
 .topbar {
  position: absolute;
  top:300/64rem;
  display: flex;
  width: 100%;
}
.topbar .item {
  flex: 1;
  text-align: center;
}
.topbar .item a{
   color: #000;
	 font-size: 25/64rem;
}
.topbar .item span {
  color: #666;
}
.topbar .item img {
  width: 65/64rem;
  height: 65/64rem;
}

 .bg{
 	background:#f8f9fa;
 	width: 100%;
 	height: 30/64rem;
  margin-top: 350/64rem;
 }
.content li{
	height:96/64rem;
	line-height: 96/64rem;
	width: 100%;
	border-bottom: 1px solid #ccc;
	font-size: 27/64rem;
	position: relative;
	
	.imgleft{
		width:67/64rem;
		height: 67/64rem;
		position: relative;
		top:20/64rem;
		left: 30/64rem;
	}
	.imgright{
		width:20/64rem;
		height:20/64rem;
		position: absolute;
		top:40/64rem;
		 right:30/64rem;
	}
	span{
		display: inline-block;
		text-indent:1.7em;
	}
	a{
		color: #000;
		font-weight: 600;
	}
}


</style>
