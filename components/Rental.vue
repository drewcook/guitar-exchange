<template>
  <div class="item-container">
    <img :src="require(`@/assets/images/${rental.image}`)" alt="Rental">
    <div class="text-container">
      <h4>{{rental.title}}</h4>
      <p>{{rental.description}}</p>
    </div>
  </div>
</template>

<script>
  export default {
    props: ['rental']
  }
</script>

<style scoped>
  .item-container {
    display: flex;
    margin: 3rem 0
  }
  .text-container {
    padding: 0 1rem
  }
  img {
    width: 17.5rem;
    border-radius: 0.5rem;
    height: 11rem
  }
  p {
    font-size: 0.8rem;
    color: grey
  }
</style>
