<template>
	<view class="content">
		<view class="text-area">
			<text class="title">123{{title}}</text>
		</view>

		<view class="">
			<u-button >默认按钮</u-button>
			<u-button type="primary" :ripple="true" ripple-bg-color="red">主要按钮</u-button>
			<u-button type="success">成功按钮</u-button>
			<u-button type="info">信息按钮</u-button>
			<u-button type="warning">警告按钮</u-button>
			<u-button type="error">危险按钮</u-button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello',
				list: [{
					text: '点赞',
					color: 'blue',
					fontSize: 28
				}, {
					text: '分享'
				}, {
					text: '评论'
				}],
				show: true
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
