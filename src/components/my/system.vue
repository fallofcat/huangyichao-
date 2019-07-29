<template>
	<div>
		<div class="header">
			 <div class="top">
				 <router-link to='/login'><img src="../../../static/img/i_back.png" alt=""></router-link>
				  <span>系统设置</span>
			 </div>
		</div>
		<div class="list">
			<ul>
				<li>
					 <span>仅在WiFi下观看和离线下载 </span> 
					  
				</li>
				<li>
					 <span>意见反馈 </span>
					 <img src="../../../static/img/i_more.png" alt="" class="imgright">
				</li>
				<li>
					 <span>关于创客学院</span> 
					  <img src="../../../static/img/i_more.png" alt="" class="imgright">
				</li>
				<li>
				    <span>当前版本</span><span class="textright">V3.1.0</span>
				</li>
			</ul>
			
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
		font-size: 34/64rem;
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
		.list {
			 
			li{
				position: relative;
				margin-top: 30/64rem;
				width: 100%;
				height: 90/64rem;
				border: 1px solid #ccc;
				line-height:90/64rem;
				font-size: 30/64rem;
				text-indent: 1em;
				color:#666;
				background:#fff;
				
				img{
					width:20/64rem;
					height:20/64rem;
					position: absolute;
					top:40/64rem;
					 right:30/64rem;
				}
				.textright{
					position: absolute;
					 right:30/64rem;
				}
			}
		}
		 
</style>
