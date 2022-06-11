<template>
  <div class="maps" id="maps">
    <h2>Our Offices</h2>
    <div class="content">
      <div class="card">
        <div class="map">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3964.5608281938075!2d3.3885197150029303!3d6.4503838257979895!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x103b8b1073ccdd79%3A0xb77c5f8bd50972a0!2s1%20Joseph%20Street%2C%20Lagos%20Island%20102273%2C%20Lagos!5e0!3m2!1sen!2sng!4v1654943829318!5m2!1sen!2sng" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
        <div class="info">
          <h4>Address</h4>
          <p>1 Joseph Street, Lagos Island 102273</p>
          <h4>Hours</h4>
          <p>Monday - Friday</p>
          <p>8am - 5pm</p>
          <h4>Contacts</h4>
          <p><a href="tel:+234 808 898 5577">+234 808 898 5577</a></p>
          <p><a href="mailto:kingsleyn24@yahoo.com">kingsleyn24@yahoo.com</a></p>
        </div>
      </div>
      <div class="card">
        <div class="map">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3964.2621849623997!2d3.330804115002993!3d6.488446825369379!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x103b8eaeb967741f%3A0x9f2b68448eafa77b!2s79%20Sanya%20St%2C%20Ijesha%20Tedo%20101241%2C%20Lagos!5e0!3m2!1sen!2sng!4v1654943894270!5m2!1sen!2sng" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
        <div class="info">
          <h4>Address</h4>
          <p>79 Sanya St, Surulere 101241.</p>
          <h4>Hours</h4>
          <p>Monday - Friday</p>
          <p>8am - 5pm</p>
          <h4>Contacts</h4>
          <p><a href="tel:+234 806 233 8622">+234 806 233 8622</a></p>
          <p><a href="mailto:tecpastryworld@gmail.com">tecpastryworld@gmail.com</a></p>
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