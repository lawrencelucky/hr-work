<template>
  <div class="jumbotron-container">
    <div class="jumbotron">
      <div class="social-media--icons">
        <img
          class="icons"
          src="../assets/icons/facebook.svg"
          alt="facebook-icon"
        />
        <img
          class="icons"
          src="../assets/icons/instagram.svg"
          alt="instagram-icon"
        />
        <img
          class="icons"
          src="../assets/icons/twitter.svg"
          alt="twitter-icon"
        />
        <img
          class="icons"
          src="../assets/icons/linkedin.svg"
          alt="linkedin-icon"
        />
      </div>
      <p class="jumbotron-text">
        We know that you are busy with deadlines and customer demands and this
        consumes all your available time and as your business expands.
      </p>
      <h1 class="jumbotron-header">We are HR Experts we can help</h1>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.jumbotron-container {
  .jumbotron {
    height: 90vh;
    display: flex;
    flex-flow: column;
    align-items: center;
    justify-content: center;
    position: relative;

    .jumbotron-text {
      font-weight: 300;
      width: 50%;
      text-align: center;
      margin-bottom: 1rem;
      color: #ffffffe4;
    }

    .jumbotron-header {
      font-size: 4rem;
      font-weight: 700;
    }

    .social-media--icons {
      display: flex;
      flex-flow: column;
      position: absolute;
      top: 48%;
      left: 4.5%;

      .icons {
        &:not(:last-child) {
          margin-bottom: 2rem;
        }
      }
    }
  }
}
</style>
