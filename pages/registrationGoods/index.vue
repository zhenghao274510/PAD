<template>
   <form @submit="formSubmit" @reset="formReset">
   	<view class="section section_gap">
   		<view class="section__title">switch</view>
   		<switch name="switch" />
   	</view>
   	<view class="section section_gap">
   		<view class="section__title">slider</view>
   		<slider name="slider" show-value></slider>
   	</view>
   	<view class="section">
   		<view class="section__title">input</view>
   		<input name="input" placeholder="please input here" />
   	</view>
   	<view class="section section_gap">
   		<view class="section__title">radio</view>
   		<radio-group name="radio-group">
   		<label>
   			<radio value="radio1" />radio1</label>
   		<label>
   			<radio value="radio2" />radio2</label>
   		</radio-group>
   	</view>
   	<view class="section section_gap">
   		<view class="section__title">checkbox</view>
   		<checkbox-group name="checkbox">
   			<label>
   				<checkbox value="checkbox1" />checkbox1</label>
   			<label>
   				<checkbox value="checkbox2" />checkbox2</label>
   		</checkbox-group>
   	</view>
   	<view class="btn-area">
   		<button formType="submit">Submit</button>
   		<button formType="reset">Reset</button>
   	</view>
   </form>
</template>
<script>
	export default {
		data() {
			return {

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
