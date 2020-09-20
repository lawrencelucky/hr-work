<template>
  <div class="blog-content-container">
    <div class="cards-container">
      <div class="top-cards">
        <div class="card-container red">
          <div class="card">
            <div class="card-head">
              <h2>Our approach</h2>
            </div>
            <div class="card-body">
              <h5>Our attention is on you!</h5>
              <p>
                Our consultancy model is intentionally small to put all the
                attention on you. We have a policy of working with very few
                clients within a certain period so you don’t have to be worry
                about feeling like a number in a crowded room.
              </p>
            </div>
          </div>
        </div>

        <div class="card-container black">
          <div class="card">
            <div class="card-head">
              <h2>Understanding of your needs</h2>
            </div>
            <div class="card-body">
              <h5>We are attentive to your needs!</h5>
              <p>
                One of our greatest strengths is the ability to listen and
                understand your employee problems and then create a tailored
                approach that will address the unique situation your business is
                facing
              </p>
            </div>
          </div>
        </div>

        <div class="card-container red">
          <div class="card">
            <div class="card-head">
              <h2>Highly skilled professionals</h2>
            </div>
            <div class="card-body">
              <h5>We have been there!</h5>
              <p>
                Because we have passed the roads before and have experience in
                managing complex employee problems. We know how to partner with
                you to make it work. We are driven by a team of well-seasoned HR
                Experts in Nigeria and led by Efeguom Oriero
              </p>
            </div>
          </div>
        </div>
      </div>

      <div class="bottom-cards">
        <div class="card-container red">
          <div class="card">
            <div class="card-head">
              <h2>
                Concerned about your <br />
                business
              </h2>
            </div>
            <div class="card-body">
              <h5>Results minded!</h5>
              <p>
                We want you to succeed, we carry you along through out the
                entire process in a timely and professional manner
              </p>
            </div>
          </div>
        </div>

        <div class="card-container black">
          <div class="card">
            <div class="card-head">
              <h2>Affordable</h2>
            </div>
            <div class="card-body">
              <h5>Highly affordable!</h5>
              <p>
                You can get AC for a fraction of the cost of an in-house HR
                Unit, but you would still receive the quality expertise you need
                at the time you need it
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.blog-content-container {
  margin-top: 4rem;

  .cards-container {
    display: grid;
    grid-gap: 3rem;

    .top-cards {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-gap: 3rem;

      @media screen and (max-width: 768px) {
        grid-template-columns: repeat(1, 1fr);
      }

      .card-container {
        padding: 3rem 4rem 4rem;
        border-radius: 5px;

        @media screen and (max-width: 425px) {
          padding: 3rem 2rem;
        }

        .card {
          color: #ffffff;

          .card-head {
            h2 {
              font-size: 2.5rem;
              font-weight: 600;
              height: 8.5rem;

              @media screen and (max-width: 768px) {
                height: auto;
                margin-bottom: 1.5rem;
              }

              @media screen and (max-width: 425px) {
                height: auto;
                margin-bottom: 1.5rem;
                font-size: 2rem;
              }
            }
          }
          .card-body {
          }
        }
      }
    }

    .bottom-cards {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      grid-gap: 3rem;

      @media screen and (max-width: 768px) {
        grid-template-columns: repeat(1, 1fr);
      }

      .card-container {
        padding: 4rem 6rem;
        border-radius: 5px;

        @media screen and (max-width: 768px) {
          padding: 3rem 4rem;
        }

        @media screen and (max-width: 425px) {
          padding: 3rem 2rem;
        }

        .card {
          color: #ffffff;

          .card-head {
            h2 {
              font-size: 2.5rem;
              font-weight: 600;
              height: 8.5rem;

              @media screen and (max-width: 768px) {
                height: auto;
                margin-bottom: 1.5rem;
              }

              @media screen and (max-width: 425px) {
                height: auto;
                margin-bottom: 1.5rem;
                font-size: 2rem;
              }
            }
          }

          .card-body {
          }
        }
      }
    }

    .red {
      background: rgba(239, 6, 51, 0.7);
    }

    .black {
      background: rgba(33, 34, 35, 0.7);
    }
  }
}
</style>
