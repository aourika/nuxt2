<template>
	<div>
		<h1>liste products</h1>
	<input type="text" v-model="ids">
	<button @click="load"> GO </button>
	</div>
</template>

<script>
export default {
	data() {
		return {
			ids: ''
		}
	},
	methods: {
		load(){
			this.$router.push('/products/'+ this.ids )

		}
	}
};
</script>