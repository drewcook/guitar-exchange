<template>
	<div class="card">
		<img :src="require(`@/assets/images/${card.image || 'eg1.jpg'}`)" alt="Electric Guitar" class="image" />
		<h3 class="header">{{ card.title }}</h3>
		<p class="snippet">{{ card.snippet }}</p>
	</div>
</template>

<script>
	export default {
		props: ['card'],
	}
</script>

<style scoped>
	.card {
		width: 31.5%;
		border: none;
		overflow: hidden;
		padding: 0;
		cursor: pointer;
	}
	.image {
		width: 25%;
		height: auto;
		margin: auto;
	}
	.header {
		font-size: 1.15rem;
		margin-top: 0.4rem;
	}
	.snippet {
		color: grey;
	}
</style>
