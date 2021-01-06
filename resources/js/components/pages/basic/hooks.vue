<template>
	<div>
		<h1 ref="myref">Hook Tutorial</h1>
		<h2>My Name Is {{ name }}</h2>
	</div>
</template>

<script>
export default {
	data(){
		return {
			name : "hendra"
		}
	},
	beforeCreate(){
		console.log(this.name);
	},
	created(){
		// console.log(this.$refs.myref)
		console.log('data and order function is avilable but not html', this.name)
	},
	mounted(){
		console.log(this.$refs.myref)
	}
}
</script>