<template>
  <section class="services">
    <h2>Quality, not quantity</h2>
    <p>We have made quality our habit. We provide a wide range of services, but they can all be summed up into this one phrase, "HELP YOU".  We strive to satisfy your business needs. Here are just a few things we do:</p>
    <div class="content">
      <Card v-for="item in data" :key="item.id" :data="item"  />
    </div>
  </section>
</template>

<script>
import Card from "../Helpers/S-Card.vue"
export default {
  components: {
    Card,
  },
  data() {
    return {
      data: [
        {
          id: 0,
          imgLink: 'https://images.unsplash.com/photo-1592963219838-6045ccbe0563',
          service: 'Export',
          desc: 'We export minerals to several countries in the west. These minerals include Zinc, Lead, Charcoal. We have an excellent track record and are trusted by many firms.'
        },
        {
          id: 1,
          imgLink: 'https://images.unsplash.com/photo-1488590528505-98d2b5aba04b',
          service: 'Web Design',
          desc: 'We partner with several web developers to help our clients build apps as quickly and as cost efficiently as possible. We help build all manner of Applications.'
        },
        {
          id: 2,
          imgLink: 'https://images.unsplash.com/photo-1521791136064-7986c2920216',
          service: 'Contracts',
          desc: 'We assist companies and governments to solve their problems quickly. Our trust worthy name makes us the choice contractor for NPA, MTN and many more.'
        },
      ]
    }
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