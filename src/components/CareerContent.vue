<template>
  <div class="career-content-container">
    <div class="news-container">
      <div class="content-container">
        <h2>Lorem ipsum dolor sit amet, consectetuer adipiscing elit</h2>
        <p>30th Oct, 2020</p>
      </div>
      <div class="image-container">
        <img src="../assets/images/careers.png" alt="careers" />
      </div>
    </div>

    <div class="news-container">
      <div class="content-container">
        <h2>Lorem ipsum dolor sit amet, consectetuer adipiscing elit</h2>
        <p>30th Oct, 2020</p>
      </div>
      <div class="image-container">
        <img src="../assets/images/careers.png" alt="careers" />
      </div>
    </div>

    <div class="news-container">
      <div class="content-container">
        <h2>Lorem ipsum dolor sit amet, consectetuer adipiscing elit</h2>
        <p>30th Oct, 2020</p>
      </div>
      <div class="image-container">
        <img src="../assets/images/careers.png" alt="careers" />
      </div>
    </div>

    <div class="news-container">
      <div class="content-container">
        <h2>Lorem ipsum dolor sit amet, consectetuer adipiscing elit</h2>
        <p>30th Oct, 2020</p>
      </div>
      <div class="image-container">
        <img src="../assets/images/careers.png" alt="careers" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.career-content-container {
  margin-top: 4rem;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-gap: 3rem;

  .news-container {
    display: flex;
    width: 50rem;

    .content-container {
      display: flex;
      flex-flow: column;
      justify-content: center;
      background: rgba(242, 242, 242, 0.3);
      padding-left: 4rem;

      h2 {
        color: #ef0633;
        font-size: 1.6rem;
        font-weight: 700;
        letter-spacing: 0;
        width: 70%;
        margin-bottom: 2rem;
      }

      p {
        color: #888888;
        font-size: 1.4rem;
        font-weight: 400;
      }
    }

    .image-container {
      img {
        width: 150px;
      }
    }
  }
}
</style>
