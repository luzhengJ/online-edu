<template>
	<view class="navBar">
		<view class="navItem" v-for="(item,index) in navList" :key="index">
			<view :class="item.icon" class="icon"></view>
			<view class="title mt-1">{{item.title}}</view>
		</view>
	</view>
</template>

<script>
	import navBarList from "../../../config/nav-bar-list.js"
	export default {
		props : {
			navList:{
				type : Array,
				default : () => navBarList()
			}
		},
		data() {
			return {
				
			};
		},
		created() {
			console.log(this.navList);
		}
	}
</script>

<style lang="scss" scoped>
 .navBar{
	width: 695rpx;
	height: 150rpx;
	 background-color: #fff;
	 margin: 50rpx auto 0;
	 display: flex;
	 justify-content: space-around;
	 align-items: center;
	 border-radius: 10rpx;
	 box-shadow: 2rpx 2rpx 5rpx #ddd;
	 .navItem{
		 display: flex;
		 flex-direction: column;
		 align-items: center;
		 .icon{
			 color: #fdc108;
			 font-size: 40rpx !important;
		 }
		 .title{
			 font-size: 12rpx;
			 color: #434851;
		 }
	 }
 }
</style>
