<template>
	<div>
		<input
			type="text"
			placeholder="URL to image"
			v-model="imageUrl" />
		<button v-on:click="$emit('adding-image', imageUrl)">Add image</button>
	</div>
</template>

<script>
export default {
	data: function() {
		return {
			imageUrl: ''
		};
	}  // data
}
</script>

<style scoped>

</style>
