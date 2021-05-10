<template>
	<header>
		<b-navbar toggleable="lg" type="dark" variant="dark">
			<div class="container">
				<b-navbar-brand href="/">Guitar Exchange</b-navbar-brand>

				<b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

				<b-collapse id="nav-collapse" is-nav>
					<b-navbar-nav>
						<b-nav-item href="/products">Products</b-nav-item>
						<b-nav-item href="/my-items">My Items</b-nav-item>
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

  #nav-collapse {
    justify-content: flex-end;
  }
</style>
