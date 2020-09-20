<template>
  <div class="career-header-container">
    <h2>Latest News</h2>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.career-header-container {
  h2 {
    font-size: 4rem;
    color: #ef0633;
    padding-bottom: 2.5rem;
    border-bottom: 0.5px solid #f99bad;
    width: 40%;

    @media screen and (max-width: 768px) {
      width: 100%;
    }

    @media screen and (max-width: 425px) {
      font-size: 3rem;
      padding-bottom: 1.5rem;
    }
  }
}
</style>
