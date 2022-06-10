<template>
  <section class="services">
    <h2>Quality, not quantity</h2>
    <p>We have made quality our habit. We provide a wide range of services, but they can all be summed up into this one phrase, "HELP YOU".  We strive to satisfy your business needs. Here are just a few things we do:</p>
    <div class="content">
      <Card  />
    </div>
  </section>
</template>

<script>
import Card from "../Helpers/S-Card.vue"
export default {
  components: {
    Card,
  }
}
</script>

<style lang="scss" scoped>
.services {
  padding: 1rem;

  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;

  h2 {
    font-size: 36px;
    font-weight: 500;
    padding: 2rem 0;
  }

  p {
    width: 600px;
    font-size: 16px;
    line-height: 1.45;
    padding: 1rem 0;
  }

  .content {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1rem;
  }

  @media screen and (max-width: $m-large) {
    .content {
      display: block;
      margin: 1rem 0;
    }
  }

  @media screen and (max-width: $medium) {
    padding: 1rem;
    display: block;

    h2 {
      font-weight: 400;
      font-size: 36px;
      padding: 1rem 0;
    }

    p {
      width: 100%;
      line-height: 1.85;
      font-size: 18px;
      padding: 1rem 0;
    }
  }
}
</style>