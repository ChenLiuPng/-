<template>
	<view>
		<!-- 顶部导航栏 -->
		<u-navbar title="" bgColor="#40ae36">
			<template #left>
				<view class="left">
					<view><u-icon name="map" color="#fff" size="20px"></u-icon></view>
					<view style="margin-left: 16rpx;margin-right: 8rpx;">海淀区中关村大厦</view>
					<view><u-icon name="arrow-down-fill" color="#fff" size="14px" :customStyle="{transform:'scale(0.6)'}"></u-icon></view>
				</view>
			</template>
			<template #right>
				<view class="right">
					<view><u-icon name="scan" color="#fff" size="25px"></u-icon></view>
					<view style="margin-left: 15rpx;"><u-icon name="chat" color="#fff" size="25px"></u-icon></view>
				</view>
			</template>
		</u-navbar>
		<!-- 搜索区域 -->
		<view class="search">
			<u-search placeholder="日照香炉生紫烟" :showAction="false" :disabled="true" @click="onSearch"></u-search>
		</view>
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
			onSearch(){
				console.log('跳转');
			}
		}
	}
</script>

<style lang="scss">
	.left {
		display: flex;
		align-items: center;
		color: #fff;
		font-size: 30rpx;
	}
	.right {
		display: flex;
	}
	.search {
		margin-top: 44px;
		padding:15rpx 26rpx;
	}
</style>
