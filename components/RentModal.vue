<template>
  <div>
    <b-button @click="showModal">Rent This Guitar</b-button>

    <b-modal ref="rent-modal" hide-footer title="Rent This Guitar">
      <div class="calendar-container">
        <div class="text-container">
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Asperiores quis soluta quia neque! Ea modi, a omnis eligendi enim ducimus asperiores. Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, autem?</p>
        </div>
          <vc-date-picker
            :value="null"
            color="indigo"
            is-dark
            is-range
          />
      </div>
      <b-button variant="outline" @click="hideModal">Order</b-button>
    </b-modal>
  </div>
</template>

<script>
export default {
  methods: {
    showModal() {
      this.$refs['rent-modal'].show()
    },
    hideModal() {
      this.$refs['rent-modal'].hide()
    },
  }
}
</script>

<style scoped>
  button {
    width: 100%;
    border: none;
    padding: 0.5rem;
    color: white;
    font-weight: 700;
    padding: 1rem 4rem;
    border-radius: 100rem;
    background-color: rgb(231, 81, 43);
    color: white;
    font-weight: 700;
    transition: 0.5s;
  }
  button.close {
    line-height: 1;
    font-size: 18px;
    border: none;
    background: none;
  }
  .calendar-container {
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
  }
  p {
    color: grey
  }
  .text-container {
    padding: 0.5rem
  }
</style>
