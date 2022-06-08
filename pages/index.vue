<template>
  <div class="home">
    <Jumbotron />
    <Services />
  </div>
</template>

<script>
import Jumbotron from "~/components/Home/Jumbotron.vue"
import Services from "~/components/Home/Services.vue"
export default {
  components: {
    Jumbotron,
    Services
  }
}
</script>

<style lang="scss" scoped>

</style>
