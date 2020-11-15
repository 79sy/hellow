<template>
	<!-- 热门课程/最新课程/名师堂 列表头-->
	<div class="listheader">
		<h3>列表头部</h3>
		<a href="#">更多</a>
	</div>
</template>

<script>
</script>

<style>
	.listheader {
		border-bottom: 2px solid #ddd;
	}
	.listheader h3{
		/* 文本粗细：加粗/取消加粗 */
		font-weight: normal;
		display: inline-block;
		/* 行内块元素与同一行中的行内元素竖直居中对齐*/
		vertical-align:middle;
		border-bottom: 2px solid #57bc4c;
		margin:0;
		padding:1.2em 1em .3em;
		/* 向下平移 */
		transform: translateY(2px);
		font-size: 1.4em;
	}
	.listheader a{
		float: right;
		margin-top: 25px;
	}
</style>
