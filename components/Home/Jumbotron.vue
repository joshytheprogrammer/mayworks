<template>
  <div class="jumbotron">
    <h1>We are committed to <br> helping you in every way.</h1>
    <p>We execute contracts, develop websites, grow brand names, export goods and so much more. Just reach out, we can find something for you.</p>
    <NuxtLink to="/quote">Get Quote</NuxtLink>
  </div>
</template>
// Fix the way this looks on mobile. Specifically the height
<style lang="scss" scoped>
.jumbotron {
  padding: 1rem;
  background-image: url("https://images.unsplash.com/photo-1617952739760-1dcae19a1d93?auto=format&fit=crop&w=1700&q=80");
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
    display: block;
    width: fit-content;
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
    background-image: url('https://images.unsplash.com/photo-1617952739760-1dcae19a1d93?auto=format&fit=crop&w=1200&q=80');
    padding-bottom: 2rem;
    height: 600px;

    h1 {
      font-weight: 400;
      font-size: 36px;
    }

    p {
      width: 100%;
      line-height: 1.85;
      font-size: 18px;
    }
  }
}
</style>