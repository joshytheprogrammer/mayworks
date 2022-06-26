<template>
  <div class="links">
    <!-- Make sure to use css to differentiate between mobile and  -->
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="/services">Services</NuxtLink>
    <NuxtLink to="/about">About</NuxtLink>
    <NuxtLink to="/contact">Contact</NuxtLink>
  </div>
</template>

<style lang="scss" scoped>
.links {
  a {
    text-decoration: none;
    color: $dark;
    cursor: pointer;

    font-weight: 400;
    font-size: 16px;

    &:hover {
      text-decoration: underline;
      text-decoration-color: $primary;
      text-underline-offset: 9px; 
    }

    &.nuxt-link-exact-active {
      text-decoration: underline;
      text-decoration-color: $primary;
      text-underline-offset: 9px; 
      color: $dark;
    }
  }

  @media screen and (min-width: $medium) {
    a {
      padding: 0 12px;
    }
  }

  @media screen and (max-width: $medium) {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    padding: 12px 0;

    a {
      padding: 15px 0;
    }
  }
}
</style>