<template>
  <nav>
    <div class="navbar">
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
          <XCircleIcon v-if="isOpen" @click="toggleMenu" />
          <MenuIcon v-else @click="toggleMenu" />
        </div>
        <!-- For Desktops -->
        <div class="desktop" v-else>
          <Menu />
        </div>
      </div>
    </div>
    <div class="menuItems" v-if="isMobile && isOpen">
      <Menu />
    </div>
  </nav>
</template>

<script>
import { MenuIcon, XCircleIcon } from '@vue-hero-icons/outline'
import Menu from "./Menu.vue"
export default {
  components: {
    Menu,
    MenuIcon,
    XCircleIcon
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
      window.innerWidth > 768 ? this.isMobile = false : this.isMobile = true
    },
    toggleMenu(){
      this.isOpen = !this.isOpen
    }
  },
}
</script>

<style lang="scss" scoped>
nav {
  padding: 14px 8px;
  position: absolute;
  top: 0;
  z-index: 12;
  width: 100%;
  background: $light;

  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 72px;

    .logo {
      width: 72px;
      
      img {
        width: 100%;
        height: 72px;
      }
    }
  }
}
</style>