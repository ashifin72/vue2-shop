<template>
  <div class="ash-catalog-item col-md-4">
    <div class="card">

      <img class="ash-catalog-item__image" :src="require('@/assets/images/' + product_data.image) " alt="img">
      <p class="ash-catalog-item__name">{{product_data.name}}</p>
      <p class="ash-catalog-item__price">Price: {{product_data.price}} грн</p>

      <button class="ash-catalog-item__add_to_cart_btn btn btn-success" @click="sendDataToParent">

        Add to cart
      </button>

    </div>

  </div>
</template>

<script>
  export default {
    name: "AshCatalogItem",

    props: {
      product_data: {
        type: Object,
        default() {
          return {}
        }
      }
    },
    data() {
      return {
        counter: 0
      }
    },
    computed: {},
    methods: {
      sendDataToParent() {
        this.$emit('sendArticle', this.product_data.article)
      }
    }
  }
</script>

<style scoped>

</style>
