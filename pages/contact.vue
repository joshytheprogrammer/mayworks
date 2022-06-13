<template>
  <div class="about">
    <form>
      <h1>Talk to us</h1>
      <div class="form-group">
        <label for="email">Email</label>
        <input class="form-control" type="text" name="email" placeholder="We'll reply to you here">
        <button class="btn" type="submit">Submit</button>
      </div>
    </form>
    <div class="map">
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3964.5608281938075!2d3.3885197150029303!3d6.4503838257979895!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x103b8b1073ccdd79%3A0xb77c5f8bd50972a0!2s1%20Joseph%20Street%2C%20Lagos%20Island%20102273%2C%20Lagos!5e0!3m2!1sen!2sng!4v1654943829318!5m2!1sen!2sng" width="100%" height="650" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.about {
  
  padding: 1rem;
  width: 100%;

  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;

  form {
    margin: 72px auto;

    h1 {
      font-size: 36px;
      font-weight: 400;
      padding: 2rem 0;
    }
    
    .form-group {

      label {
        display: block;
        text-transform: uppercase;
        font-weight: 500;
        font-size: 12px;
        padding: 0.2rem 0 0.2rem 0;
      }

      .form-control {
        display: block;
        width: 480px;
        height: 48px;
        background: $grey;
        color: $dark;
        border: none;
        outline: 1px solid $dark;
        border-radius: 4px;
        padding: 0 0 0 0.2rem;
        margin-bottom: 1rem;
        transition: background .2s linear, outline .1s ease-in-out;
        
        font-size: 16px;
        font-weight: 400;

        &:focus {
          outline: 2px solid $dark;
          background: $light;
        }
      }

      .btn {
        display: block;
        background: $primary;
        color: $light;
        border: none;
        font-size: 16px;
        font-weight: 400;
        border-radius: 4px;
        height: fit-content;
        width: fit-content;
        padding: 8px 12px;
        margin: 1rem 0;
        cursor: pointer;
        transition: box-shadow .2s ease-in-out, padding .2s linear;

        &:hover {
          box-shadow: 0px 8px 8px $dark;
          padding: 9px 16px;
        }

        &:disabled {
          cursor: not-allowed;
          opacity: .6;
        }
      }
    }
  }

  @media screen and (max-width: $medium) {
    display: block;

    form {
      margin-bottom: 72px;
      h1 {
        text-align: left;
      }

      .form-group {
        .form-control {
          width: 100%;
        }
      }
    }
  }
}
</style>