<template>
  <div class="jumbotron">

  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.jumbotron {
  padding: 1rem;
  background-image: url("https://images.unsplash.com/photo-1597334948330-38795f25d05d?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1700&q=80");
  background-attachment: fixed;
  background-repeat: no-repeat;
  object-fit: fill;
  height: 1200px;
  max-width: 100%;
  color: $light;

  @media screen and (max-width: $medium) {
    max-height: 800px;
  }
}
</style>