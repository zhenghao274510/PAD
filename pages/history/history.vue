<template>
	<view>
		<page-heade :title="title"></page-heade>
		<view class="uni-his-swiper">
			<view class="uni-his-item">
				<view class="uni-his-left ">
					<view class="uni-his-left-list uni-bor-bottom">
						<view class="uni-his-left-list-one">
							AWB
						</view>
						<view class="uni-his-left-list-two ">
							AWB002
						</view>
					</view>
					<view class="uni-his-left-list uni-bor-bottom">
						<view class="uni-his-left-list-one">
							AWB
						</view>
						<view class="uni-his-left-list-two">
							AWB002
						</view>
					</view>
					<view class="uni-his-left-list uni-bor-bottom">
						<view class="uni-his-left-list-one">
							AWB
						</view>
						<view class="uni-his-left-list-two">
							AWB002
						</view>
					</view>
					<view class="uni-his-left-list uni-bor-bottom">
						<view class="uni-his-left-list-one">
							AWB
						</view>
						<view class="uni-his-left-list-two">
							AWB002
						</view>
					</view>
					<view class="uni-his-left-list">
						<view class="uni-his-left-list-one">
							AWB
						</view>
						<view class="uni-his-left-list-two">
							AWB002
						</view>
					</view>
				</view>
				<view class="uni-his-right uni-bor-left">
					<view class="uni-his-right-top">
						<image src="/static/image/history.png" mode=""></image>
					</view>
					<view class="uni-his-right-top uni-bor-top" @click="showMore=!showMore">
						<image src="/static/image/history_up.png" mode="" v-if="showMore"></image>
						<image src="/static/image/history_down.png" mode="" v-else></image>
					</view>
				</view>
			</view>
			<view class="uni-his-item">
				<view class="uni-his-left ">
					<view class="uni-his-left-list uni-bor-bottom">
						<view class="uni-his-left-list-one">
							AWB
						</view>
						<view class="uni-his-left-list-two ">
							AWB002
						</view>
					</view>
					<view class="uni-his-left-list uni-bor-bottom">
						<view class="uni-his-left-list-one">
							AWB
						</view>
						<view class="uni-his-left-list-two">
							AWB002
						</view>
					</view>
					<view class="uni-his-left-list uni-bor-bottom">
						<view class="uni-his-left-list-one">
							AWB
						</view>
						<view class="uni-his-left-list-two">
							AWB002
						</view>
					</view>
					<view class="uni-his-left-list uni-bor-bottom">
						<view class="uni-his-left-list-one">
							AWB
						</view>
						<view class="uni-his-left-list-two">
							AWB002
						</view>
					</view>
					<view class="uni-his-left-list" v-if="showMore">
						<view class="uni-his-left-list-one">
							AWB
						</view>
						<view class="uni-his-left-list-two">
							AWB002
						</view>
					</view>
				</view>
				<view class="uni-his-right uni-bor-left">
					<view class="uni-his-right-top">
						<image src="/static/image/history.png" mode=""></image>
					</view>
					<view class="uni-his-right-top uni-bor-top" @click="showMore=!showMore">
						<image src="/static/image/history_up.png" mode="" v-if="showMore"></image>
						<image src="/static/image/history_down.png" mode="" v-else></image>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import pageHeade from "@/components/page-head.vue"
	export default {
		data() {
			return {
				showMore: false,
				title: "历史查询"
			}
		},
		components: {
			pageHeade
		},
		methods: {
			onClick() {
				this.$emit('click')
			}
		}
	}
</script>

<style lang="scss">
	@charset "UTF-8";
	.uni-his-swiper {
		width: 90%;
		margin: 0 auto;
	}
	.uni-his-item {
		background: $uni-bg-color;
		border-radius: $uni-border-radius-lg;
		box-shadow: 0 0 4px 4px rgb(238, 237, 237);
		display: flex;

	}

	.uni-his-left {
		flex: 1;
		padding: 0 25px;
	}

	.uni-his-right {
		padding: 0 15px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.uni-his-right image {
		width: 30px;
		height: 30px;
	}

	.uni-his-right-top {
		display: flex;
		flex: 1;
		justify-content: center;
		align-items: center;
		height: 50%;
	}

	.uni-his-left-list-one {
		font-weight: bold;
		color: #333;
	}

	.uni-his-left-list-two {
		font-weight: bold;
		color: #999;
	}
</style>
