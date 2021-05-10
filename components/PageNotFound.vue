<template>
	<div class="centered">
		<h1>Page not found.</h1>
		<p>Looks like you struck a bad chord.</p>
		<b-button><nuxt-link to="/">Go Back</nuxt-link></b-button>
	</div>
</template>

<script>
	export default {}
</script>

<style scoped>
	.centered {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	h1 {
		margin-top: 5rem;
	}

	a {
		text-decoration: none;
		color: #fff;
	}
</style>
