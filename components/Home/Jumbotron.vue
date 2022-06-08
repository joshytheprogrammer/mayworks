<template>
  <div class="jumbotron">
    <h1>We are committed to <br> helping you in every way.</h1>
    <p>We execute contracts, develop websites, grow brand names, export goods and so much more. Just reach out, we can find something for you.</p>
    <NuxtLink to="/quote">Get Quote</NuxtLink>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.jumbotron {
  padding: 1rem;
  background-image: url("https://images.unsplash.com/photo-1597334948330-38795f25d05d?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1700&q=80");
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-color: $dark;
  object-fit: fill;
  height: 700px;
  max-width: 100%;
  color: $light;

  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;

  h1 {
    font-weight: 500;
    font-size: 48px;
    padding: 1rem 0;
  }

  p { 
    width: 380px;
    line-height: 1.875;
    font-size: 18px;
    padding: 1rem 0;
  }

  a {
    background: $light;
    color: $primary;
    padding: 12px 16px;
    text-decoration: none;
    border-radius: 8px;

    &:hover {
      background: $primary;
      color: $light;
    }
  }

  @media screen and (max-width: $medium) {
    max-height: 800px;
  }
}
</style>