<template>
	<div>
		<h1> A single user, with IDs: {{ $route.params.id }} </h1>
	</div>
</template>		


<script>
	export default {
	validate (data) {
		return /^\d+$/.test(data.params.id)
	}
};
</script>