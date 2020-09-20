<template>
  <div id="contact" class="footer-container">
    <div class="chat-us-container">
      <div class="chat-us-content">
        <h2>Chat with Us</h2>
      </div>
      <div class="image-container">
        <img src="../assets/icons/chat-with-us.svg" alt="" />
      </div>
    </div>
    <div class="content">
      <div class="logo-container">
        <img
          src="../assets/icons/hr-work-logo-light.svg"
          alt="hr-work-logo-light"
        />
      </div>
      <div class="nav">
        <ul>
          <li class="nav-list"><a href="#about" class="nav-link">About</a></li>
          <li class="nav-list none">|</li>
          <li class="nav-list">
            <a href="#packages" class="nav-link">Packages</a>
          </li>
          <li class="nav-list none">|</li>
          <li class="nav-list"><a href="#blog" class="nav-link">Blog</a></li>
          <li class="nav-list none">|</li>
          <li class="nav-list">
            <a href="#careers" class="nav-link">Careers</a>
          </li>
          <li class="nav-list none">|</li>
          <li class="nav-list">
            <a href="#contact" class="nav-link">Contact</a>
          </li>
        </ul>
      </div>
      <div class="contact-us">
        <h2>Contact Us</h2>
        <p>
          11 Deji Olamiju Street, <br />
          Soluyi-Gbagada, Lagos <br />
          Call: 07034417961 <br />
          Email: info@alphaduxcnsulting.com
        </p>
      </div>
      <div class="copyright">
        <p>&copy; 2020 HR Work All right reserved</p>
      </div>
      <div class="terms-and-conditions">
        <p>Terms & Conditions | Privacy Policy</p>
      </div>
      <div class="social-media--icons">
        <img class="icon" src="../assets/icons/facebook.svg" alt="facebook" />
        <img class="icon" src="../assets/icons/instagram.svg" alt="instagram" />
        <img class="icon" src="../assets/icons/twitter.svg" alt="twitter" />
        <img class="icon" src="../assets/icons/linkedin.svg" alt="linkedin" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.footer-container {
  background: #ef0633;
  padding: 10rem 10rem 5rem 10rem;
  position: relative;

  @media screen and (max-width: 1024px) {
    padding: 10rem 1rem 5rem 1rem;
  }

  @media screen and (max-width: 768px) {
    padding: 7rem 5rem 2rem 5rem;
  }

  @media screen and (max-width: 425px) {
    padding: 5rem 1rem 3rem;
  }

  .chat-us-container {
    position: absolute;
    display: flex;
    margin-right: 10rem;
    right: 0%;
    top: -2.5rem;
    background: #ffffff;
    padding: 0.4rem 0.4rem 0.4rem 1.5rem;
    border-radius: 10rem;
    box-shadow: 0px 6px 15px rgba(71, 5, 7, 0.25);

    @media screen and (max-width: 768px) {
      margin-right: 4rem;
    }

    @media screen and (max-width: 425px) {
      padding-left: 0.4rem;
    }

    @media screen and (max-width: 320px) {
      margin-right: 2rem;
    }

    .chat-us-content {
      display: flex;
      align-items: center;
      margin-right: 1rem;

      h2 {
        color: #ef0633;
        font-size: 1.6rem;
      }

      @media screen and (max-width: 425px) {
        display: none;
      }
    }
    .image-container {
      background-color: #ef0633;
      padding: 1rem;
      border-radius: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
    }
  }

  .content {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-row-gap: 7rem;

    @media screen and (max-width: 768px) {
      grid-template-columns: repeat(1, 1fr);
      justify-items: center;
      grid-row-gap: 4rem;
    }

    @media screen and (max-width: 425px) {
      grid-row-gap: 2rem;
      justify-items: flex-start;
    }

    .logo-container {
      img {
        width: 15rem;

        @media screen and (max-width: 425px) {
          width: 12rem;
        }
      }
    }

    .nav {
      color: #ffffff;
      justify-self: center;

      @media screen and (max-width: 768px) {
        order: 1;
      }

      @media screen and (max-width: 425px) {
        justify-self: flex-start;
      }

      ul {
        display: flex;

        @media screen and (max-width: 425px) {
          display: flex;
          flex-flow: column;
          align-items: flex-start;
        }

        .nav-list {
          list-style: none;

          &:not(:last-child) {
            margin-right: 2rem;

            @media screen and (max-width: 425px) {
              margin-right: 0;
            }
          }

          .nav-link {
            text-decoration: none;
            color: #ffffff;
            font-size: 1.2rem;
            font-weight: 600;

            @media screen and (max-width: 425px) {
              font-size: 1.4rem;
            }
          }
        }

        .none {
          @media screen and (max-width: 425px) {
            display: none;
          }
        }
      }
    }

    .contact-us {
      color: #ffffff;
      justify-self: end;

      @media screen and (max-width: 768px) {
        justify-self: center;
        order: 2;
      }

      @media screen and (max-width: 425px) {
        justify-self: flex-start;
      }

      h2 {
        text-align: right;
        font-size: 2rem;
        font-weight: 600;
        margin-bottom: 1rem;

        @media screen and (max-width: 768px) {
          text-align: center;
        }

        @media screen and (max-width: 425px) {
          text-align: left;
        }
      }

      p {
        text-align: right;
        font-size: 1.4rem;
        font-weight: 300;
        line-height: 2.5rem;

        @media screen and (max-width: 768px) {
          text-align: center;
        }

        @media screen and (max-width: 425px) {
          text-align: left;
        }
      }
    }

    .copyright {
      color: #ffffff;
      font-size: 1.4rem;

      @media screen and (max-width: 768px) {
        order: 4;
      }
    }

    .terms-and-conditions {
      color: #ffffff;
      font-size: 1.4rem;
      justify-self: center;

      @media screen and (max-width: 768px) {
        order: 5;
      }

      @media screen and (max-width: 425px) {
        justify-self: flex-start;
      }
    }

    .social-media--icons {
      justify-self: end;

      @media screen and (max-width: 768px) {
        justify-self: center;
        order: 3;
      }

      @media screen and (max-width: 425px) {
        justify-self: flex-start;
      }

      .icon {
        &:not(:last-child) {
          margin-right: 2rem;
        }
      }
    }
  }
}
</style>
