<template>
	<view class='uni-flex uni-column uni-align-center uni-padding-wrap'>
		<view class="uni-flex uni-inline-item">
			<image src="/static/logo.png" mode="" class="image-view"></image>
		</view>
		<form @submit="formSubmit" @reset="formReset" class="uni-padding-wrap">
			<view class="section uni-flex uni-inline-item uni-input-row">
				<view class="section__title">input</view>
				<input class="bottom-border" name="input" type="text" placeholder="请输入账号" v-model="acount" />
			</view>
			<view class="section uni-flex uni-inline-item uni-input-row">
				<view class="section__title">input</view>
				<input class="bottom-border" name="input" type="password" placeholder="请输入密码" v-model="pwd" />
			</view>
			<view class="btn-area">
				<button formType="submit" type="primary" style="color: #FFFFFF;border-radius: 20px;background: orange;">登录</button>
			</view>
			<view class="uni-flex uni-inline-item uni-align-center uni-common-mt">
				<radio-group name="radio-group">
					<label v-for="(v,k) in checkboxList" :key="k">
						<checkbox :value="v.value" />{{v.name}}</label>
				</radio-group>
			</view>

		</form>
	</view>
</template>
<script>
	export default {
		data() {
			return {
				acount: '',
				pwd: '',
				checkboxList: [{
						name: '仓库管理PDA',
						value: "radio1"
					},
					{
						name: '叉车平板电脑',
						value: "radio2"
					}
				]
			};
		},
		//监听属性 类似于data概念
		computed: {},
		//监控data中的数据变化
		watch: {},
		//import引入的组件需要注入到对象中才能使用
		components: {

		},
		onLoad() {

		},
		//方法集合
		methods: {}
	}
</script>
<style scoped lang="scss">

</style>
