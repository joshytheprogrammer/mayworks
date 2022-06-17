<template>
  <div class="card">
    <img :src="data.imgLink" loading="lazy" :alt="data.service + ' image on mayworks'">
    <div class="details">
      <h2>{{data.service}}</h2>
      <p>{{data.desc}}</p>
      <button>Contact us</button>
      <!-- Be sure to turn button into a link that leads to mayworks email -->
    </div>
  </div>
</template>

<script>
export default {
  props: ['data']
}
</script>

<style lang="scss" scoped>
.card {
  margin: 72px 0;
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

      &:hover {
        background-image: linear-gradient(rgba(0, 0, 0, 0.4) 0 0);
      }
    }
  }

  @media screen and (max-width: $m-large) {
    margin: 2rem 0;
  }

}
</style>