<template>
  <section class="testimonials" id="testimonials">
    <h2>Here's what our clients say</h2>
    <div class="content">
      <div class="card">
        <p class="testimony">”Every day, they strive to improve their service to the clients by developing the right blend of technology and creativity to make sure every job done is done as efficiently as possible.”</p>
        <h4 class="testifier">-Ikenna Isiadinso</h4>
      </div>
      <div class="card">
        <p class="testimony">"Mayworks partnered with joshytheprogrammer.com to assist clients in building their personal portfolios and they were very happy with the results. Thank you mayworks"</p>
        <h4 class="testifier">-Nsofor Joshua</h4>
      </div>
      <div class="card">
        <p class="testimony">"My company has been partnered with Mayworks for over three years now, Mayworks has assisted us in, Cleaning our Windows (SkyScraper), Advertising on Billboards, Installating Computer resources and much more"</p>
        <h4 class="testifier">-Aghaduno Okechukwu</h4>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.testimonials {
  margin: 72px 1rem;

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
    gap: 1rem;
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