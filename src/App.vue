<template>
  <div id="app">
    <div id="nav" class="ash-nav">
      <router-link  to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
</template>
<script>


  export default {
    name: 'app',
    components: {

    }
  }
</script>
<style lang="sass">
/*@import "assets/sass/main"*/
</style>
