<template>
	<view class="optionTab">
		<view class="tabItem" v-for="(item,index) in tabList" :key="index">
			<view class="ele" v-for="(ele,i) in item" :key="i">
				<view class="left">
					<text :class="ele.icon" class="icon"></text>
					<text class="title">{{ele.title}}</text>
				</view>
				<view class="right">
					<text class="rightIcon"></text>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import optionTabList from "../../../config/option-list.js"
	export default {
		props : {
			tabList : {
				type : Array,
				default : () => optionTabList()
			}
		},
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style lang="scss" scoped>
   .optionTab{
	   margin-top: 80rpx;
	   padding: 0 56rpx;
	   .tabItem{
		 .ele{
			 display: flex;
			 justify-content: space-between;
			 align-items: center;
			 border-bottom: 1rpx solid #eee;
			 line-height: 117rpx;
			 // padding-right: 40rpx;
			 &:last-child{
			 	border: 0;
			 }
			 .left{
				 display: flex;
				 align-items: center;
				 .icon{
					font-size: 35rpx;
					 color: #2b8ff5;
				 }
				 .title{
					 display: inline-block;
					 font-size: 32rpx;
					 color:#64696b;
					 margin-left: 20rpx;
				 }
			 }
			 .right{
				 .rightIcon{
				     &::after{
				 		content: "";
				 		display: inline-block;
				 		width: 20rpx;
				 		height: 20rpx;
				 		border-right:4rpx solid #ccc;
				 		border-bottom:4rpx solid #ccc;
				 		transform: rotate(-45deg);
						font-size: 32rpx;
				 	}	
				 }
			 }
		 }
	   }
   }
</style>
