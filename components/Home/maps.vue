<template>
  <div class="maps" id="maps">
    <h2>Our Offices</h2>
    <div class="content">
      <div class="card">
        <div class="map">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3964.142733117981!2d3.349837015003017!3d6.503609225197974!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x103b8d8b74245bed%3A0x98cda859077b56f4!2sTrack%20IT!5e0!3m2!1sen!2sng!4v1654336974311!5m2!1sen!2sng" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
        <div class="info">
          <h4>Address</h4>
          <p>40, Oyekan Street Off Ogunlana Drive Surulere, Lagos.</p>
          <h4>Hours</h4>
          <p>Monday - Friday</p>
          <p>8am - 5pm</p>
          <h4>Contacts</h4>
          <p><a href="tel:+234 901 563 0453">+234 901 563 0453</a></p>
          <p><a href="mailto:info@trackit.com.ng">info@trackit.com.ng</a></p>
        </div>
      </div>
      <div class="card">
        <div class="map">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15759.903889839848!2d7.455027980789247!3d9.06595313563224!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x104e0b146aaaaaab%3A0x1f731775230620f7!2sTrack%20IT%20Limited!5e0!3m2!1sen!2sng!4v1654354352329!5m2!1sen!2sng" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
        <div class="info">
          <h4>Address</h4>
          <p>Suite 11b, DBM plaza Wuse Zone1, Abuja.</p>
          <h4>Hours</h4>
          <p>Monday - Friday</p>
          <p>8am - 5pm</p>
          <h4>Contacts</h4>
          <p><a href="tel:+234 802 317 8729">+234 802 317 8729</a></p>
          <p><a href="mailto:info@trackit.com.ng">info@trackit.com.ng</a></p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.maps {
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
    grid-template-columns: 1fr 1fr;
    width: 80%;

    .card {
      margin: 1rem 0;

      .map {
        width: 100%;
      }

      .info {
        padding: 1rem 0;

        h4 {
          font-weight: 500;
          padding: 0.9rem 0;
        }

        p {
          padding: 0.5rem 0;

          a {
            color: $dark;
          }
        }
      }
    }
  }

  @media screen and (max-width: $m-large) {
    .content {
      width: 90%;
      display: block; 
    }
  }

  @media screen and (max-width: $medium) {
    .content {
      width: 100%;
    }
  }
}
</style>