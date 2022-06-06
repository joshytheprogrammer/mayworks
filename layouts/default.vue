<template>
  <div class="app">
    <Nav />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
import Nav from "~/components/App/Nav.vue"
import Footer from "~/components/App/Footer.vue"
export default {
  components: {
    Nav,
    Footer
  }
}
</script>

<style>

</style>