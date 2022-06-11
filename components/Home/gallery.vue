<template>
  <section class="gallery">
    <figure>
      <img src="https://assets.zyrosite.com/cdn-cgi/image/format=auto,w=1200,h=992,fit=crop/mPoyZVg96EI62K0E/joel-filipe-unsplash-A83b6wlplpfyBgkr.jpg" alt="">
    </figure>
    <figure>
      <img src="https://assets.zyrosite.com/cdn-cgi/image/format=auto,w=1200,h=992,fit=crop/mPoyZVg96EI62K0E/joel-filipe-unsplash-A83b6wlplpfyBgkr.jpg" alt="">
    </figure>
    <figure>
      <img src="https://assets.zyrosite.com/cdn-cgi/image/format=auto,w=1200,h=992,fit=crop/mPoyZVg96EI62K0E/joel-filipe-unsplash-A83b6wlplpfyBgkr.jpg" alt="">
    </figure>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.gallery {
  padding: 1rem;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;

  figure {


    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block; 
    }
  }
}
</style>