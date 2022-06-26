<template>
  <div class="home">
    <Jumbotron />
    <Services />
    <Gallery />
    <Testimonials />
    <Maps />
  </div>
</template>

<script>
import Jumbotron from "~/components/Home/Jumbotron.vue"
import Services from "~/components/Home/Services.vue"
import Gallery from "~/components/Home/gallery.vue"
import Testimonials from "~/components/Home/testimonial.vue"
import Maps from "~/components/Home/maps.vue"

export default {
  components: {
    Jumbotron,
    Services,
    Gallery,
    Testimonials,
    Maps
  }
}
</script>