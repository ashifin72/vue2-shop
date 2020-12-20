<template>
  <div class="v-main-wrapper container-fluid">
    <h2>Hello 123</h2>
    <div class="container">
      <ash-catalog/>
      <ash-cart/>

    </div>

  </div>

</template>

<script>
  import AshCatalog from "./catalog/AshCatalog";
  import AshCart from "./cart/AshCart";
  export default {

    name: "AshWraper",
    components:{
      AshCatalog,
      AshCart
    }
  }
</script>

<style scoped>

</style>
