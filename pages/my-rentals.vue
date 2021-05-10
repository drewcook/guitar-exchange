<template>
	<div>
		<h1>My Rentals</h1>
    <Rental v-for="rental in myRentals" :key="rental.id" :rental="rental" />
	</div>
</template>

<script>
  import { mapState } from 'vuex'
	export default {
		layout: 'no-nav',
    computed: {
      ...mapState(['myRentals'])
    }
	}
</script>
