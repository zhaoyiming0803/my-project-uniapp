<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view>
			<text class="title">{{title}}</text>
		</view>
	</view>
</template>

<script>
	import AuthingMove from './bundle'
	// import { test } from './test'

	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {
			// test(0)
			// console.log('----------: ', uni instanceof Proxy)
			// uni.setStorageSync('storage_key', 'hello');
			// uni.showToast({
			// 	title: 'title123',
			// 	icon: 'success',
			// 	duration: 3000
			// })

			console.log('AuthingMove:::::: ', Object.keys(AuthingMove))

			// AuthingMove.setStorageSync('a1b2', 'a1b2')

			my.setStorage({
				key: '123321',
				data: '123321'
			})
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
		margin: 200rpx auto 50rpx auto;
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
