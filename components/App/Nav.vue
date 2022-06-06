<template>
  <nav class="navbar">
    <!-- The Logo Section -->
    <div class="logo">
      <NuxtLink to="/">
        <img src="../../assets/images/mayworks-logo.png" alt="Mayworks Logo">
      </NuxtLink>
    </div>
    <!-- The Menu Section -->
    <div class="menu">
      <!-- For Phones -->
      <div class="mobile" v-if="isMobile">
        <MenuIcon @click="toggleMenu" />
        <Menu v-if="isOpen" />
      </div>
      <!-- For Desktops -->
      <div class="desktop" v-else>
        <Menu />
      </div>
    </div>
  </nav>
</template>

<script>
import { MenuIcon } from '@vue-hero-icons/outline'
import Menu from "./Menu.vue"
export default {
  components: {
    Menu,
    MenuIcon
  },
  data(){
    return {
      isMobile: '',
      isOpen: false,
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
    },
    toggleMenu(){
      this.isOpen = !this.isOpen
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