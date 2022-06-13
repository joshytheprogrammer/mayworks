<template>
  <div class="about">
    <div class="content">
      <div class="img">
        <img src="https://images.unsplash.com/photo-1618470554490-6fee45d9c2ac?auto=format&fit=crop&w=1200&h=992" alt="">
      </div>
      <div class="details">
        <h1>The company Mayworks</h1>
        <p>Mayworks was found in 2014 for the sole purpose of exporting minerals from Nigeria to other countries in the world namely the US, UK, China, Canada and more. Fast forward a few years and now Mayworks is dedicated to helping small and big businesses solve problems.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.about {
  margin: 72px 0;
  padding: 1rem;

  .content {
    display: grid;
    gap: 1rem;
    grid-template-columns: 1fr 1fr;

    .details {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;

      h1 {
        font-size: 36px;
        font-weight: 500;
        padding: 2rem 0;
      }

      p {
        font-size: 16px;
        line-height: 1.85;
        padding: 1rem 0;
      }
    }

    .img {
      width: 100%;
      max-height: 100%;

      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }
  }

  @media screen and (max-width: $medium) {
    .content {
      display: block;
    }
  }
}
</style>