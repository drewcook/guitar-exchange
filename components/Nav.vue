<template>
	<header>
		<b-navbar toggleable="lg" type="dark" variant="dark">
			<div class="container">
				<b-navbar-brand><nuxt-link to="/">Guitar Exchange</nuxt-link></b-navbar-brand>

				<b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

				<b-collapse id="nav-collapse" is-nav>
					<b-navbar-nav>
						<nuxt-link to="/products" class="nav-link"><b-nav-text>Products</b-nav-text></nuxt-link>
						<nuxt-link to="/my-items" class="nav-link"><b-nav-text>My Items</b-nav-text></nuxt-link>
					</b-navbar-nav>
				</b-collapse>
			</div>
		</b-navbar>
	</header>
</template>

<script>
	export default {}
</script>

<style scoped>
	header {
		margin-bottom: 50px;
	}

	.navbar-brand a {
		text-decoration: none;
		color: #fff;
	}

	#nav-collapse {
		justify-content: flex-end;
	}

	.nav-link {
		text-decoration: none;
	}

	.nav-link .navbar-text {
		color: #fff;
	}
</style>
