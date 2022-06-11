<template>
  <section class="gallery">
    <figure>
      <img src="https://assets.zyrosite.com/cdn-cgi/image/format=auto,w=1200,h=992,fit=crop/mPoyZVg96EI62K0E/joel-filipe-unsplash-A83b6wlplpfyBgkr.jpg" alt="">
    </figure>
    <figure>
      <img src="https://assets.zyrosite.com/cdn-cgi/image/format=auto,w=1200,h=1120,fit=crop/mPoyZVg96EI62K0E/Mask-Group-Yr0xLlkMbXcjQxwK.png" alt="">
    </figure>
    <figure>
      <img src="https://assets.zyrosite.com/cdn-cgi/image/format=auto,w=1200,h=1376,fit=crop/mPoyZVg96EI62K0E/leo-manjarrez-unsplash-YZ4enVpOejhVw2aW.jpg" alt="">
    </figure>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.gallery {
  margin: 2rem 0;
  padding: 1rem;
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