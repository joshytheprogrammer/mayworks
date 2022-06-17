<template>
  <div class="services">
    <div class="service" v-for="item in data" :key="item.id">
      <div class="_image">
        <img :src="item.imgLink" :alt="item.service">
      </div>
      <div class="_details">
        <h2>{{item.service}}</h2>
        <p>{{item.desc}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return {
      data: [
        {
          id: 0,
          imgLink: 'https://images.unsplash.com/photo-1598193957011-39b9f2916992?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1080&q=80',
          service: 'Export',
          desc: 'We export minerals to several countries in the west. These minerals include Zinc, Lead, Charcoal. We have an excellent track record and are trusted by many firms.'
        },
        {
          id: 1,
          imgLink: 'https://images.unsplash.com/photo-1467232004584-a241de8bcf5d?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1080&q=80',
          service: 'Web Design',
          desc: 'We partner with several web developers to help our clients build apps as quickly and as cost efficiently as possible. We help build all manner of Applications.'
        },
        {
          id: 2,
          imgLink: 'https://images.unsplash.com/photo-1598061349464-e28ba5710d26?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1080&q=80',
          service: 'Contracts',
          desc: 'We assist companies and governments to solve their problems quickly. Our trust worthy name makes us the choice contractor for NPA, MTN and many more.'
        },
        {
          id: 3,
          imgLink: 'https://images.unsplash.com/photo-1503694978374-8a2fa686963a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1080&q=80',
          service: 'Printing',
          desc: 'We assist companies and governments in printing anything and everything they need. This includes T-Shirts, Logos, Banners, Hats, etc'
        },
      ]
    }
  }
}
</script>
<style lang="scss" scoped>
.service {
  padding: 1rem;

  display: grid;
  gap: 1rem;
  grid-template-columns: 1fr 1fr;

  ._image {
    max-width: 100%;
    height: 600px;

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }

  ._details {
    padding: 1rem;
    width: 100%;
    display: flex;
    text-align: center;
    flex-direction: column;
    justify-content: center;

    h2 {
      font-size: 36px;
      font-weight: 400;
      padding-bottom: 1rem;
    }

    p {
      font-size: 16px;
      line-height: 1.85;
      padding: 1rem 0;
    }
  }

  @media screen and (max-width: $medium) {
    display: block;

    ._image {
      max-width: 90%;
      height: 400px;
      margin: auto;
    }
  }
}
</style>