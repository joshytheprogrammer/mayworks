<template>
  <section class="testimonials">
    <h2>Here's what our clients say</h2>
    <div class="content">
      <div class="card">
        <p class="testimony">"Track IT is a very innovative company with a great vision for future of Nigeria."</p>
        <h4 class="testifier">-Ikenna Isiadinso</h4>
      </div>
      <div class="card">
        <p class="testimony">"Track IT is the best software licensing company to work with and also the best company to get technology skills and certifications that will promote your tech career. The best place to learn is at Track IT."</p>
        <h4 class="testifier">-Oluwatosin Ajayi</h4>
      </div>
      <div class="card">
        <p class="testimony">"Every day, they strive to improve their service to the clients by developing the right blend of technology and creativity to make sure every job done is done as efficiently as possible."</p>
        <h4 class="testifier">-Claurice Turner</h4>
      </div>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.testimonials {
  padding: 1rem;

  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;

  h2 {
    font-size: 36px;
    font-weight: 400;
    padding: 2rem 0;
  }

  .content {
    display: grid;
    gap: 12px;
    grid-template-columns: repeat(3, 1fr);

    .card {
      margin: 2rem 0;

      .testimony {
        font-size: 16px;
        line-height: 1.85;
      }

      .testifier{
        font-size: 14px;
        font-weight: 500;
        padding: 1rem 0;
      }
    }
  }

  @media screen and (max-width: $m-large) {
    .content {
      grid-template-columns: repeat(2, 1fr);
      margin: 1rem 0;
    }
  }

  @media screen and (max-width: $medium) {
    .content {
      display: block;
    } 
  }
}
</style>