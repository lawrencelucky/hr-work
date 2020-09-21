<template>
  <div class="packages-content-container">
    <div class="main-content">
      <div class="cards-container">
        <div class="card-container">
          <div class="card">
            <div class="card-head">
              <div class="category blue">
                <p>Retainership Category</p>
              </div>
            </div>
            <div class="card-body">
              <h2>HR Remote Manager</h2>
              <p class="price">₦3,480</p>
              <p class="stages">Basic, Bronze, Foundation</p>
              <button class="btn">Add to Cart</button>
            </div>
          </div>
        </div>

        <div class="card-container">
          <div class="card">
            <div class="card-head">
              <div class="category red">
                <p>Retainership Category</p>
              </div>
            </div>
            <div class="card-body">
              <h2>HR Remote Manager</h2>
              <p class="price">₦3,480</p>
              <p class="stages">Basic, Bronze, Foundation</p>
              <button class="btn">Add to Cart</button>
            </div>
          </div>
        </div>

        <div class="card-container">
          <div class="card">
            <div class="card-head">
              <div class="category green">
                <p>Retainership Category</p>
              </div>
            </div>
            <div class="card-body">
              <h2>HR Remote Manager</h2>
              <p class="price">₦3,480</p>
              <p class="stages">Basic, Bronze, Foundation</p>
              <button class="btn">Add to Cart</button>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="button-container">
      <button class="btn">
        View more packages
        <img class="image" src="../assets/icons/polygon.svg" alt="" />
      </button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.packages-content-container {
  display: flex;
  flex-flow: column;
  align-items: center;

  .main-content {
    .cards-container {
      margin-top: 5rem;
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-gap: 7rem;
      justify-items: center;

      @media screen and (max-width: 768px) {
        grid-template-columns: repeat(1, 1fr);
      }

      @media screen and (max-width: 1024px) {
        grid-gap: 2rem;
      }

      .card-container {
        .card {
          width: 32rem;
          box-shadow: rgba(136, 136, 136, 0.25) 0px 6px 15px;
          border-radius: 1.5rem;

          @media screen and (max-width: 960px) {
            width: 30rem;
          }

          @media screen and (max-width: 768px) {
            width: 40rem;
          }

          @media screen and (max-width: 425px) {
            width: 38rem;
          }

          @media screen and (max-width: 375px) {
            width: 32rem;
          }

          @media screen and (max-width: 320px) {
            width: 28rem;
          }

          .card-head {
            background-image: url('https://res.cloudinary.com/ddu7ud0f0/image/upload/v1600687726/package_iabsfd.png');
            height: 25rem;
            background-repeat: no-repeat;
            background-size: cover;
            background-position: top;
            border-top-left-radius: 1.5rem;
            border-top-right-radius: 1.5rem;
            position: relative;

            .category {
              position: absolute;
              top: 15%;
              padding: 0.8rem 1.5rem;
              border-top-right-radius: 2rem;
              border-bottom-right-radius: 2rem;

              p {
                color: #ffffff;
                font-size: 1.3rem;
                font-weight: 600;
              }
            }

            .blue {
              background: #0057da;
            }

            .red {
              background: #ef0633;
            }

            .green {
              background: #00ba34;
            }
          }

          .card-body {
            display: flex;
            flex-flow: column;
            align-items: center;

            h2 {
              font-size: 1.6rem;
              font-weight: 600;
              color: #565656;
              margin-top: 5rem;

              @media screen and (max-width: 375px) {
                font-size: 1.4rem;
              }
            }

            .price {
              color: #ef0633;
              font-size: 3rem;
              font-weight: 700;
              margin-top: 1rem;

              @media screen and (max-width: 375px) {
                font-size: 2.2rem;
              }
            }

            .stages {
              color: #888888;
              font-weight: 600;
              margin-top: 1rem;
            }

            .btn {
              margin-top: 2rem;
              margin-bottom: 3rem;
              padding: 1.5rem 7rem;
              border: 2px solid #888888;
              background-color: #ffffff;
              font-size: 1.6rem;
              color: #888888;
              border-radius: 10rem;
              cursor: pointer;

              @media screen and (max-width: 375px) {
                padding: 1rem 4rem;
                font-size: 1.4rem;
              }

              &:focus {
                outline: 0;
              }
            }
          }
        }
      }
    }
  }

  .button-container {
    margin-top: 8rem;

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
}
</style>
