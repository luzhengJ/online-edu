<template>
	<view class="my">
		<view class="userinfo">
			<!-- 个人信息 -->
			<user-info></user-info>
			<!-- 导航 -->
			<nav-bar></nav-bar>
		
		</view>
		<!-- 选项菜单栏 -->
		<option-tab></option-tab>
	</view>
</template>

<script>
	import userInfo from "./components/user-info.vue"
	import navBar from "./components/navBar.vue"
	import optionTab from "./components/optionTab.vue"
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		},
		components:{
			userInfo,
			navBar,
			optionTab
		}
	}
</script>

<style lang="scss" scoped>
   Page,.my{
	   height: 100%;
	   background-color: #fff;
   }
   .userinfo{
	   height: 320rpx;
	   background-color: #5ccc84;
	   padding: 20rpx;
	   border-radius: 0 0 48rpx 48rpx;
   }
</style>
