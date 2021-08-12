<template>
  <div>
      <header>
          <h2> App Header</h2>
          <p>items: {{cartCount}}</p>
      </header>
  </div>
</template>

<script>
export default {
    computed: {
        cartCount() {
            return this.$store.state.cartItems
        }
    },
}
</script>

<style>
div {
    text-align: center;
}
header {
    width: full;
    display: flex;
    height: 5em;
    background-color: #5CDB95;
    color: #05386B;
    font-size: 2em;
    display: flex;
    align-items: center;
    justify-content: center;
}
p {
    margin-left: 4em;
}
</style>