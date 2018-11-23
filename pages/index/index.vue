<template>
	<view>
		<uni-richtext :richList.sync="richList" :uploadUrl="uploadUrl"></uni-richtext>
	</view>
</template>

<script>
	import uniRichtext from '../../components/uni-richtext.vue'
	export default {
		components:{
			uniRichtext
		},
		data() {
			return {
				richList: [],
				uploadUrl:"http://120.78.87.84:8080/conduit/file/uploadFile"
			}
		},
		watch:{
			richList:function (newValue,oldValue) {
				console.log(newValue)
			}
		}
	}
</script>

<style>
</style>
