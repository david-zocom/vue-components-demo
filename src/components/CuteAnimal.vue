<template>
	<div>
		<img v-bind:src="url" />
	</div>
</template>

<script>
export default {
	props: ['url']
}
</script>

<style scoped>
div {
	background-color: white;
}
img {
	width: 200px;
	height: auto;
}
</style>
