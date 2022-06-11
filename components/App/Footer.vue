<template>
  <footer>
    <div class="address">
      <h3>Address</h3>
      <p>1 Joseph Street, Lagos Island 102273</p>
      <p>79 Sanya St, Surulere 101241.</p>
    </div>
    <div class="contacts">
      <h3>Contacts</h3>
      <p>+234 808 898 5577</p>
      <p>+234 806 233 8622</p>
      <p><a href="mailto:kingsleyn24@yahoo.com">kingsleyn24@yahoo.com</a></p>
    </div>
    <div class="attribution">
      <h3>Mayworks Integrated Limited</h3>
      <p>This website was created by <a href="https://www.joshytheprogrammer.com">joshytheprogrammer</a></p>
      <p>© 2022 Mayworks Integrated Limited. All Rights Reserved.</p>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  margin: 72px 0;
  padding: 0 1rem;

  text-align: center;

  display: grid;
  grid-template-columns: repeat(3, 1fr);

  div {
    padding: 1rem 0;
  }

  h3 {
    font-size: 24px;
    font-weight: 500;
  }

  p {
    font-size: 14px;
    font-weight: 400;
    padding: 5px 0;
  }

  a {
    color: $dark;
  }

  @media screen and (max-width: $m-large) {
    display: block;
  }
}
</style>