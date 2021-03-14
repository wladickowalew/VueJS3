<style scoped>
	h1{
		color: blue;
	}
</style>

<template>
	<div>
		<h1>{{ msg }}</h1>
	</div>
</template>

<script>
	module.exports = {
		data:function () {
			return{
				msg: "Hello, component!"
			};
		}
	};
</script>