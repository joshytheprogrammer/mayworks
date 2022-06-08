<template>
  <div class="services">
    <h2 class="_s_head">Quality, not quantity</h2>
    <p class="_s_desc">We have made quality our habit. We provide a wide range of services, but they can all be summed up into this one phrase, "HELP YOU".  We strive to satisfy your business needs. Here are just a few things we do:</p>
    <div class="content">
      <div class="card">
        <img src="https://images.unsplash.com/photo-1592963219838-6045ccbe0563" alt="">
        <div class="details">
          <h2>Export</h2>
          <p>We export minerals to several countries in the west. These minerals include Zinc, Lead, Charcoal. We have an excellent track record and are trusted by many firms.</p>
          <button>Contact us</button>
        </div>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1488590528505-98d2b5aba04b" alt="">
        <div class="details">
          <h2>Web Design</h2>
          <p>We partner with several web developers to help our clients build apps as quickly and as cost efficiently as possible. We help build all manner of Applications.</p>
          <button>Contact us</button>
        </div>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1521791136064-7986c2920216" alt="">
        <div class="details">
          <h2>Contracts</h2>
          <p>We assist companies and governments to solve their problems quickly. Our trust worthy name makes us the choice contractor for NPA, MTN and many more.</p>
          <button>Contact us</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.services {
  padding: 1rem;

  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;

  ._s_head {
    font-size: 36px;
    font-weight: 500;
    padding: 2rem 0;
  }

  ._s_desc {
    width: 600px;
    font-size: 16px;
    line-height: 1.45;
    padding: 1rem 0;
  }

  .content {
    display: flex;
    justify-content: space-evenly;

    .card {
      max-width: 400px;
      padding: 1rem;

      img {
        width: 100%;
        
        object-fit: contain;
      }

      .details {
        padding: 0.5rem 0;
        text-align: center;

        h2 {
          font-size: 32px;
          font-weight: 500;
        }

        p {
          font-size: 14px;
          padding: 1.9rem 0;
          line-height: 1.7;
        }

        button {
          padding: 12px 16px;
          background: $primary;
          cursor: pointer;
          border: none;
          width: fit-content;
          height: fit-content;
          border-radius: 4px;
        }
      }
    }
  }
}
</style>