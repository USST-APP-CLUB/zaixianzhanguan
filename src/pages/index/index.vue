
<template>
	<view class="content">
		<image class="logo" src="/static/logo.png" />
		<!-- 这里完全可以不用a标签 -->
		<a @click="open(1)"></a>
		<a @click="open(2)" ></a>
		<a @click="open(3)"></a>
		<a @click="open(4)"></a>
		<a @click="open(5)"> </a>
		<a @click="open(6)"> </a>
		
		<view>
			<!-- <div class="title">{{title}}</div>0 -->
			<!-- <router-link to="/pages/list/list">跳转到列表页</router-link> -->
		</view>
		<view>  
                
        </view>  
	</view>
</template>


<script>
	export default {
		data() {
			return {
			}
		},
		onLoad() {

		},
		methods: {
			open(type){
				if(type==1){
					HWH5.openWebview({uri:"https://shlgwm.usst.edu.cn/12149/list.htm"})
				}
				else if(type==2){
					HWH5.openWebview({uri:"https://shlgwm.usst.edu.cn/12150/list.htm"})
				window.location.href=""
				}
				else if(type==3){
					HWH5.openWebview({uri:"https://shlgwm.usst.edu.cn/12151/list.htm"})
				window.location.href=""
				}
				else if(type==4){
					HWH5.openWebview({uri:"https://shlgwm.usst.edu.cn/12152/list.htm"})
				}
				else if(type==5){
					HWH5.openWebview({uri:"https://shlgwm.usst.edu.cn/12153/list.htm"})
				}
				else if(type==6){
					HWH5.openWebview({uri:"https://shlgwm.usst.edu.cn/12154/list.htm"})
				}

			}
		}
	}
</script>
<style>
	.content {
		text-align: center;
		height: 100%;
	}

	.logo {
		height: 100%;
		width:750upx;
		position: absolute;
		top:0;
		left: 0;
		
	}

	.content a:nth-of-type(1){
		width: 15%;
		height: 10%;
		/* background: #fff; */
		position: absolute;
		left: 10%;
		top: 20%;
	}

	.content a:nth-of-type(2){
		width: 15%;
		height: 10%;
		/* background: #fff; */
		position: absolute;
		left: 35%;
		top: 30%;
	}

	.content a:nth-of-type(3){
		width: 15%;
		height: 10%;
		/* background: #fff; */
		position: absolute;
		left: 49%;
		top: 43%;
	}

		.content a:nth-of-type(4){
		width: 15%;
		height: 10%;
		/* background: #fff; */
		position: absolute;
		left: 49%;
		top: 59%;
	}

	.content a:nth-of-type(5){
		width: 15%;
		height: 10%;
		/* background: #fff; */
		position: absolute;
		left: 35%;
		top: 74%;
	}


	.content a:nth-of-type(6){
		width: 15%;
		height: 10%;
		/* background: #fff; */
		position: absolute;
		left: 10%;
		top: 83%;
	}

	.title {
		
		font-size: 36upx;
	}
	.skip {
		margin-top: 20upx;
	}
</style>
