<template>
	<view class="uni-content">
		<uni-gird columnNum="2" :options="options"></uni-gird>
	</view>
</template>

<script>
	import uniGird from "@/components/uni-grid/uni-grid.vue"
	export default{
		data(){
			return{
				options:[]
			}
		},
		components:{
			uniGird
		},
		onLoad(){
			
		}
	}
</script>

<style>
</style>
