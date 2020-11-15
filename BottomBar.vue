<template>
	<div class="bottombar">
		<div class="container">
			<!-- 服务列表 -->
			<div class="servicelist">
				<div class="services">
					<div class="service">
						<h3>关于i前端</h3>
						<ul>
							<li><a href="#">发展历程</a></li>
							<li><a href="#">管理团队</a></li>
							<li><a href="#">企业文化</a></li>
							<li><a href="#">加入我们</a></li>
						</ul>
					</div>
					<div class="service">
						<h3>新手帮助</h3>
						<ul>
							<li><a href="#">学员帐号</a></li>
							<li><a href="#">选课流程</a></li>
							<li><a href="#">网报流程</a></li>
							<li><a href="#">上课地点</a></li>
						</ul>
					</div>
					<div class="service">
						<h3>常见问题</h3>
						<ul>
							<li><a href="#">如何注册</a></li>
							<li><a href="#">如何搜课</a></li>
							<li><a href="#">如何报名</a></li>
							<li><a href="#">如何缴费</a></li>
						</ul>
					</div>
					<div class="service">
						<h3>联系我们</h3>
						<ul>
							<li><a href="#">校区电话</a></li>
							<li><a href="#">意见建议</a></li>
							<li><a href="#">联系邮箱</a></li>
						</ul>
					</div>
				</div>
				
				<div class="hotline">
					<div class="left"> <!--left高度为100px,而电话图标只有40px-->
						<span class="phone"></span> <!--使用span显示图片，而不是.left-->
					</div>
					<div class="right">
						<div>客服热线</div>		
						<div>4008-220-220(9:00 - 24：00)</div>		
					</div>
				</div>
			</div>
			<!-- 版权声明 -->
			<div class="zdb">
				<div class="s">
					Copyright © 2016 iqianduan.com, All Rights Reserved 版权所有
				</div>
				<div class="x">
					北京前端教育科技有限公司　京ICP备123456号-1 京公网安备110180201608号
				</div>
				
			</div>
			
		</div>
	</div>
</template>

<script>
</script>

<style>
	.bottombar{
		background: #eee;
		border: 1px solid #ddd;
	}
	.servicelist{
		display: flex;
	}
	.servicelist .services{
		flex: 615;
		display: flex;
	}
	
	.servicelist .services .service{
		flex: 1;
	}
	.servicelist .hotline{
		flex: 385;
		display: flex;
	}
	
	.servicelist .hotline .left{
		flex:100;
		padding: 50px 0 0 60px ;
	}
	.servicelist  .hotline  .left .phone{
		/* 显示精灵图中的一部分 */
		display: inline-block;
		width: 40px;
		height: 40px;
		background-image:url(../assets/img/iconlist.png);
		background-position:0 -410px;
	}
	.servicelist .hotline .right{
		font-size:1.3em ;
		flex:285 ;
		padding: 40px 0 0 0px ;
	}
	.bottombar   .zdb{
		text-align: center;
		color: #999;
		padding: 8px 0;
		border-top: 1px solid #ddd;
		line-height: 20px;
	}
</style>
