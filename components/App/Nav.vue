<template>
  <div class="navbar">
    <div class="logo">
      <NuxtLink to="/">
        <img src="../../assets/images/mayworks-logo.png" alt="Mayworks Logo">
      </NuxtLink>
    </div>
    <div class="menu">
      <div class="mobile" v-if="isMobile">
        <Menu />
      </div>
      <div class="desktop" v-else>
        <Menu />
      </div>
    </div>
  </div>
</template>

<script>
import Menu from "./Menu.vue"
export default {
  components: {
    Menu
  },
  data(){
    return {
      isMobile: ''
    }
  },
  mounted() {
    this.checkMobile()
    window.addEventListener("resize", this.checkMobile);
  },
  unmounted() {
    window.removeEventListener("resize", this.checkMobile);
  },
  methods: {
    checkMobile() {
      window.innerWidth >= 768 ? this.isMobile = false : this.isMobile = true
      // console.log(this.isMobile)
    }
  },
}
</script>

<style lang="scss" scoped>
.navbar {
  .logo {

  }
}
</style>