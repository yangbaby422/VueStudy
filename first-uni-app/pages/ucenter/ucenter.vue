<template>
	<view class="content">
		<view>
			<text class="title">{{name}}</text>
			<navigator url="setting" hover-class="navigator-hover">
				<button type="primary">个人设置<tton>
			</navigator>
		<view>
		<view>
</template>

<script>
	export default {
		data() {
			return {
				name: '洋酱'
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
		text-align: center;
		height: 400upx;
	}
	.title {
		font-size: 36upx;
		color: #8f8f94;
	}
	
</style>