<template>
  <div class="card">
    <img src="https://images.unsplash.com/photo-1521791136064-7986c2920216" loading="lazy" alt="">
    <div class="details">
      <h2>Contracts</h2>
      <p>We assist companies and governments to solve their problems quickly. Our trust worthy name makes us the choice contractor for NPA, MTN and many more.</p>
      <button>Contact us</button>
    </div>
  </div>
  <!-- <div class="card">
        <img src="https://images.unsplash.com/photo-1488590528505-98d2b5aba04b" loading="lazy" alt="">
        <div class="details">
          <h2>Export</h2>
          <p>We export minerals to several countries in the west. These minerals include Zinc, Lead, Charcoal. We have an excellent track record and are trusted by many firms.</p>
          <button>Contact us</button>
        </div>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1488590528505-98d2b5aba04b" loading="lazy" alt="">
        <div class="details">
          <h2>Web Design</h2>
          <p>We partner with several web developers to help our clients build apps as quickly and as cost efficiently as possible. We help build all manner of Applications.</p>
          <button>Contact us</button>
        </div>
      </div> -->
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.card {
  width: 100%;

  img {
    width: 100%;
    height: 400px;
    object-fit: cover;
  }

  .details {
    padding: 0.5rem 0;

    h2 {
      font-size: 36px;
      font-weight: 400;
    }

    p {
      font-size: 16px;
      line-height: 1.85;
      padding: 1rem 0;
    }

    button {
      padding: 12px 16px;
      background: $primary;
      color: $light;
      cursor: pointer;
      border: none;
      font-size: inherit;
      border-radius: 4px;
    }
  }
}
</style>