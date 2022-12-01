<template>
	<view class="info">
		<!-- 头部 -->
		<view class="top">
			<view class="left">
				<image src="../../../static/微信图片_20221031192140.jpg" mode=""></image>
			</view>
			<view class="right">
				<view class="name">立即登录</view>
				<view class="text">登录解锁更多功能</view>
			</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss">
   .info{
	   display: flex;
	   justify-content: space-between;
	   align-items: center;
	   margin-top: 35rpx;
	   margin-left: 20rpx;
	   .top{
		   display: flex;
		   align-items: center;
		   .left{
			   width: 125rpx;
			   height: 125rpx;
			   image{
				   width: 100%;
				   height: 100%;
				   border-radius: 50%;
			   }
		   }
		   .right{
			   display: flex;
			   flex-direction: column;
			   margin-left: 20rpx;
			   .name{
				   margin-bottom: 10rpx;
				   color: #eef9f1;
				   font-size: 32rpx;
			   }
			   .text{
				   color: #eef9f1;
				   font-size: 26rpx;
			   }
		   }
	   }
   }
</style>
