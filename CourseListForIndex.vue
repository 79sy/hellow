<template>
	<div class="courselist">
		<div class="container">
			<!-- 头部 -->
			<ListHeaderForIndex></ListHeaderForIndex>
			<!-- 课程列表 -->
			<div class="courses">
				<div class="course">
					<div class="picbox"><img class="pic" src="../assets/img/course/01.jpg" ></div>
					<a href="#"><div class="title">12-微信小程序开发</div></a>
					<div class="tname">讲师：程涛</div>
					<div class="price">￥599.00</div>
				</div>
				<div class="course">
					<div class="picbox"><img class="pic" src="../assets/img/course/02.jpg" ></div>
					<a href="#"><div class="title">12-微信小程序开发</div></a>
					<div class="tname">讲师：程涛</div>
					<div class="price">￥599.00</div>
				</div>
				<div class="course">
					<div class="picbox"><img class="pic" src="../assets/img/course/03.jpg" ></div>
					<a href="#"><div class="title">09-UI基础组件</div></a>
					<div class="tname">讲师：纪迎新</div>
					<div class="price">￥299.00</div>
				</div>
				<div class="course">
					<div class="picbox"><img class="pic" src="../assets/img/course/04.jpg" ></div>
					<a href="#"><div class="title">03-小程序进阶开发</div></a>
					<div class="tname">讲师：李然</div>
					<div class="price">￥499.00</div>
				</div>
			</div>			
		</div>
	</div>
</template>

<script>
	import ListHeaderForIndex from'./ListHeaderForIndex.vue'
	export default{
		// 主策当前组件中可以使用的子组件
		components:{ListHeaderForIndex}
	}
	
</script>

<style>
	.courselist{
		background: #fcfcfc;
	}
	.courses {          /*课程列表*/
		display: flex;
	}
	.courses  .course{		/*一个课程*/
		flex: 1;
		padding: 20px;
	}
	.courses  .course:first-child {
		padding-left: 0;
	}
	.courses  .course:last-child {
		padding-right: 0;
	}
	.courses  .course  .pic{
		width: 100%; /*控制图片的尺寸刚好占满父容器*/
		transition: all .3;  /*渐变动画*/
	}
    .courses .course .pic:hover{
		cursor: pointer;
		transform: scale(1.2);   /*缩放变形*/
	}
	.courses  .course  .picbox{
		/*容器中的内容溢出后如何处理 :隐藏*/
		overflow: hidden;
	}
	.courses .course  .title{
		font-size:16px;
	}
	.courses .course  .price{
		font-size:18px;
		color: #FF6600;
	}
	
</style>
