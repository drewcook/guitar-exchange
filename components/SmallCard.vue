<template>
	<nuxt-link :to="`/products/${card.id}`" class="card-container">
		<img
			:src="require(`@/assets/images/${card.image || 'eg1.jpg'}`)"
			alt="Electric Guitar"
			class="image"
		/>
	</nuxt-link>
</template>

<script>
	export default {
		props: ['card'],
	}
</script>

<style scoped>
	.card-container {
		width: 24%;
		border: 1px solid #ccc;
		padding: 10px;
		border-radius: 0.5rem;
		overflow: hidden;
		margin-bottom: 1.5rem;
		cursor: pointer;
	}

	.image {
		display: block;
		width: 25%;
		height: auto;
		margin: auto;
	}
</style>
