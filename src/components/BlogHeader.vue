<template>
  <div class="blog-header-container">
    <p>We bring a wealth of local market knowledge...</p>
    <h2>Why HR Work</h2>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.blog-header-container {
  color: #ffffff;

  p {
    font-size: 1.5rem;
    margin-bottom: 1rem;

    @media screen and (max-width: 425px) {
      font-size: 1.3rem;
    }
  }

  h2 {
    font-size: 4rem;

    @media screen and (max-width: 425px) {
      font-size: 3rem;
    }
  }
}
</style>
