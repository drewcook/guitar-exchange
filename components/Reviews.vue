<template>
  <div class="reviews">
    <h3>Customer Reviews</h3>
    <p v-if="$fetchState.pending">Loading...</p>
    <p v-else-if="$fetchState.error">An error occurred :(</p>
    <div v-else>
      <div v-if="reviews.results">
        <Review v-for="review in reviews.results" :key="review.id.value" :review="review" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      reviews: null
    }
  },
  async fetch() {
    this.reviews = await fetch('https://randomuser.me/api?results=5').then(res => res.json())
  }
}
</script>

<style>

</style>
