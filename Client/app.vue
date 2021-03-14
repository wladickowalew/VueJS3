<template>
	<div>
		Hello World!
		<c-tag></c-tag>
		<p><input type="text" v-model="message"></p>
		<par-cap v-bind:p-text="message" 
		         v-on:update="receive"></par-cap>
	</div>
</template>

<script>
	let Header = require("./header.vue");
	let ParCap = require("./par-cap.vue");
	module.exports = {
		components:{
			cTag: Header,
			parCap: ParCap
		},
		methods: {
        	receive: function(value){
        		this.message = value;
        	}
		},
		data: function () {
				return {message: "Hello!"}
			}
	};
</script>