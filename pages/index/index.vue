<template>
	<view class="container">
		<view style="padding: 15rpx;">
			<swiper class="banner swiper" indicator-dots circular easing-function="linear">
				<swiper-item wx:for="{{array}}">
					<view style="width: 100%;">
						<image class="banner" mode=" aspectFit " src="{{item}}"></image>
					</view>
				</swiper-item>
			</swiper>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				href: 'https://uniapp.dcloud.io/component/README?id=uniui'
			}
		},
		methods: {

		}
	}
</script>

<style>
	.container {
		padding: 20px;
		font-size: 14px;
		line-height: 24px;
	}

	.swiper .wx-swiper-dot.wx-swiper-dot-active {
		width: 25rpx;
		height: 10rpx;
		background: rgb(0, 0, 0);
		border-radius: 25rpx;
	}
</style>
