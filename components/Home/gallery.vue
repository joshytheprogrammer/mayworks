<template>
  <section class="gallery" id="gallery">
    <figure>
      <img src="../../assets/images/zinc.jpg" alt="zinc">
    </figure>
    <figure>
      <img src="../../assets/images/lead.jpg" alt="lead">
    </figure>
    <figure>
      <img src="../../assets/images/charcoal.jpg" alt="charcoal">
    </figure>
  </section>
</template>

<style lang="scss" scoped>
.gallery {
  margin: 72px 1rem;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;

  figure {
    height: 400px;

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block; 
    }
  }

  @media screen and (max-width: $m-large) {
    grid-template-columns: repeat(2, 1fr);
  }

  @media screen and (max-width: $medium) {
    display: block;
    
    figure {
      margin: 1rem 0;
    }
  }
}
</style>