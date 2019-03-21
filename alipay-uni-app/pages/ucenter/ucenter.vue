<template>
	<view class="content">
		<view class="top">
			<view class="title">
				<text>{{title}}</text>
			</view>
			<view class="set">
				<text>{{setting}}</text>
			</view>
		</view>

		<view class="infor">
			<image src="../../static/avatar.jpg"></image>
			<text class="username">{{username}}</text>
			<text class="mobile">{{mobile}}</text>
		</view>

		<view class="item" v-for="(user,index) in users" :key="index">
			<image :src="user.avatar" mode=""></image>
			<view class="right">{{user.name}}</view>
		</view>

	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '我的',
				setting: '设置',
				username: '洋酱',
				mobile: '18761672058',
				avatar: 'avatar.jpg',
				users: [{
						name: '支付宝会员',
						avatar: '../../static/huiyuan.png'
					},
					{
						name: '商家服务',
						avatar: '../../static/service.png'
					},
					{
						name: '账单',
						avatar: '../../static/zhangdan.png'
					},
					{
						name: '公益',
						avatar: '../../static/gongyi.png'
					},
					{
						name: '余额',
						avatar: 'static/yue.png'
					},
					{
						name: '余额宝',
						avatar: 'static/yuebao.png'
					},
					{
						name: '银行卡',
						avatar: 'static/yinhangka.png'
					},
					{
						name: '芝麻信用',
						avatar: 'static/zhimaxinyong.png'
					},
					{
						name: '蚂蚁借呗',
						avatar: 'static/mayijiebei.png'
					}
				]


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

	.top {
		display: flex;
		background: #2F85FC;
		justify-content: space-between;
	}

	.infor {
		border-top: 50upx solid #2F85FC;
		display: flex;
		height: 150upx;
		width: 100%;
		background: #2F85FC;

	}

	.infor image {
		margin-left: 30upx;
		width: 120upx;
		height: 120upx;
	}

	.username {
		margin-top: 10upx;
		margin-left: 50upx;
	}

	.mobile {
		margin-top: 50upx;
		margin-left: -80upx;
	}

	.item {
		width: 100%;
		display: flex;
		height: 100upx;

		border: 1upx solid #eee;
		margin-right: 20upx;
		margin-bottom: 10upx;
		background-color: #fff;
		padding-left: 5upx;
		padding-right: 5upx;
		padding-top: 5upx;
	}

	.item image {
		height: 50upx;
		width: 50upx;
		margin-top: 40upx;
	}

	.right {
		margin-left: 20upx;
		margin-top: 50upx;
	}
</style>
