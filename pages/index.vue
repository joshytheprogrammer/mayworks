<template>
  <div class="home">
    <Jumbotron />
    <Services />
    <Gallery />
  </div>
</template>

<script>
import Jumbotron from "~/components/Home/Jumbotron.vue"
import Services from "~/components/Home/Services.vue"
import Gallery from "~/components/Home/gallery.vue"

export default {
  components: {
    Jumbotron,
    Services,
    Gallery
  }
}
</script>

<style lang="scss" scoped>

</style>
