<template>
  <div class="who-we-are-content-container">
    <div class="main-content">
      <div class="left-content">
        <div class="text-container">
          <p class="paragraph-one">
            HR Work is an advisory firm with strong competence and experience in
            providing Human Resources Retainership Services to small or medium
            sized organisations.
          </p>
          <p class="paragraph-two">
            We know that you are busy with deadlines and customer demands and
            this consumes all your available time and as your business expands,
            your employee challenges begin to multiply and then problems with
            hiring, setting and measuring performance, policies for direction
            among others become more evitable.
          </p>
        </div>
        <div class="card-container">
          <div class="card">
            <h3>Our Mission:</h3>
            <p>
              To make HR Systems work for Small to Medium sized companies.
            </p>
          </div>
          <div class="card">
            <h3>Our Vision:</h3>
            <p>
              To be the HR retainership firm of choice to thriving businesses
            </p>
          </div>
        </div>
      </div>
      <div class="right-content">
        <div class="image-container">
          <img
            class="image"
            src="https://res.cloudinary.com/ddu7ud0f0/image/upload/v1600687728/who-we-are_g9drwf.png"
            alt="who-are-img"
          />
        </div>
      </div>
    </div>
    <div class="button-container">
      <button class="btn">
        Discover more
        <img class="image" src="../assets/icons/polygon.svg" alt="" />
      </button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.who-we-are-content-container {
  .main-content {
    display: flex;
    margin-top: 4.5rem;

    @media screen and (max-width: 768px) {
      display: flex;
      flex-flow: column;
    }

    @media screen and (max-width: 425px) {
      margin-top: 3rem;
    }

    .left-content {
      .text-container {
        width: 90%;
        color: #565656;

        @media screen and (max-width: 768px) {
          width: 100%;
        }

        .paragraph-one {
          margin-bottom: 3rem;
          font-weight: 400;
        }

        .paragraph-two {
          font-weight: 400;
        }
      }

      .card-container {
        display: grid;
        grid-template-columns: repeat(2, 22rem);
        grid-gap: 10rem;
        margin-top: 5rem;

        @media screen and (max-width: 1024px) {
          grid-gap: 5rem;
          margin-top: 3rem;
        }

        @media screen and (max-width: 768px) {
          justify-content: center;
          margin-bottom: 3rem;
          margin-top: 4rem;
        }

        @media screen and (max-width: 425px) {
          grid-template-columns: repeat(1, 1fr);
          margin-top: 3rem;
          grid-gap: 3rem;
        }

        .card {
          background: rgba(249, 155, 173, 0.5);
          color: #ef0633;
          width: 252px;
          height: 154px;
          padding: 3rem;

          @media screen and (max-width: 1024px) {
            width: 200px;
            padding: 2rem;
          }

          @media screen and (max-width: 768px) {
            width: 220px;
          }

          @media screen and (max-width: 425px) {
            width: 100%;
            height: auto;
          }

          h3 {
            margin-bottom: 0.5rem;
          }

          p {
            font-size: 1.5rem;
            font-weight: 600;
            line-height: 2.3rem;
            letter-spacing: 0.5px;

            @media screen and (max-width: 425px) {
              font-size: 1.3rem;
            }
          }
        }
      }
    }

    .right-content {
      .image-container {
        @media screen and (max-width: 768px) {
          display: flex;
          justify-content: center;
        }

        .image {
          width: 50rem;

          @media screen and (max-width: 960px) {
            width: 45rem;
          }

          @media screen and (max-width: 425px) {
            width: 38rem;
          }

          @media screen and (max-width: 375px) {
            width: 35rem;
          }

          @media screen and (max-width: 320px) {
            width: 28rem;
          }
        }
      }
    }
  }

  .button-container {
    margin-top: 4rem;

    .btn {
      padding: 1.2rem 4rem 1.2rem 2rem;
      background: #ef0633;
      color: #ffffff;
      font-weight: 600;
      font-size: 1.5rem;
      text-align: center;
      border: 0;
      border-radius: 5px;
      box-shadow: 0 6px 15px rgba(233, 40, 45, 0.25);
      cursor: pointer;
      position: relative;

      .image {
        position: absolute;
        right: 6%;
        top: 32%;
      }
    }
  }

  @media screen and (max-width: 768px) {
    display: flex;
    flex-flow: column;
    align-items: center;
  }
}
</style>
