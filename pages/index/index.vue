<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {
			console.log("index load")
		},
		onShow() {
			console.log("index show")
		},
		onTabItemTap(e) {
			console.log(e)
		},
		methods: {

		}
	}
</script>

<style lang="scss">
  $small-height: 220rpx;
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;

		.logo {
			height: $small-height;
			width: $small-height;
			margin-top: $small-height;
			margin-left: auto;
			margin-right: auto;
			margin-bottom: 50rpx;
		}

		.text-area {
			display: flex;
			justify-content: center;

			.title {
				font-size: 36rpx;
				color: #8f8f94;
			}
		}
	}
</style>
