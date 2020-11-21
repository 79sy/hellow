<template>
		<div class="menulist">
			<div class="container">
				<h1>一花，一灯，一盏茶</h1>
				<h1>食饮，食酒，食朋友</h1>
				<ul>
					<li class="menu" v-for="m of menulist">
						<div class="tu">
							<img class="pic" :src="require('../assets/'+m.pic)">
						</div>
						<h1>{{m.mname}}</h1>
						<div class="inContainer">
							<span>{{m.introduce}}</span>
						</div>
						<div>
							<a :href="m.herf">了解更多</a>
						</div> 
					</li>
				</ul>
			</div>
		</div>
	
</template>

<script>
	export default{
		//1
		//2
		data(){
			return{
				menulist:[
					{
						pic:'img/chinese.jpg',
						mname:'中式菜品',
						introduce:'中式烹调技艺在漫长的历史发展过程当中,融合了各民族的智慧与文化。',
						herf:'https://www.baidu.com/',
					},
					{
						pic:'img/chinese.jpg',
						mname:'西式菜品',
						introduce:'中式烹调技艺在漫长的历史发展过程当中,融合了各民族的智慧与文化。',
						herf:'https://www.baidu.com/',
					},
					{
						pic:'img/chinese.jpg',
						mname:'中式菜品',
						introduce:'中式烹调技艺在漫长的历史发展过程当中,融合了各民族的智慧与文化。',
						herf:'https://www.baidu.com/',
					},
					],
			}
		},
		//3
	}
	
</script>

<style>
	.menulist{

	}
	.menulist ul {
		display: flex;
		list-style: none;
	}
	.menulist li{
		flex: 1;
	}
	.menulist  h1{
		margin: 30px;
		font-weight: 600;
		text-align: center;
	}
	.menulist .inContainer{
		width: 200px;
		height: 100px;
		margin-left: auto;
		margin-right: auto;
		
	}
	.menulist span{
		display: block;
		color:#888;
		text-align: center;
	}
	.menulist a{
		display: block;
		text-align:center;
	}
	.menulist  .tu{
		overflow: hidden;
		text-align: center;
	}
	.menulist .pic {
		transition: all  .3s;	/*渐变动画*/
	}
	.menulist .pic:hover {
		/* transform: scale();	/*变形：缩放*/ 
		 transform: scale(1.1); 
		cursor: pointer;
	}
</style>
