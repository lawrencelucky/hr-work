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
          <li class="nav-list">|</li>
          <li class="nav-list">
            <a href="#packages" class="nav-link">Packages</a>
          </li>
          <li class="nav-list">|</li>
          <li class="nav-list"><a href="#blog" class="nav-link">Blog</a></li>
          <li class="nav-list">|</li>
          <li class="nav-list">
            <a href="#careers" class="nav-link">Careers</a>
          </li>
          <li class="nav-list">|</li>
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

    .chat-us-content {
      display: flex;
      align-items: center;
      margin-right: 1rem;

      h2 {
        color: #ef0633;
        font-size: 1.6rem;
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

    .nav {
      color: #ffffff;
      justify-self: center;

      ul {
        display: flex;

        .nav-list {
          list-style: none;

          &:not(:last-child) {
            margin-right: 2rem;
          }

          .nav-link {
            text-decoration: none;
            color: #ffffff;
            font-size: 1.2rem;
            font-weight: 600;
          }
        }
      }
    }

    .contact-us {
      color: #ffffff;
      justify-self: end;

      h2 {
        text-align: right;
        font-size: 2rem;
        font-weight: 600;
        margin-bottom: 1rem;
      }

      p {
        text-align: right;
        font-size: 1.4rem;
        font-weight: 300;
        line-height: 2.5rem;
      }
    }

    .copyright {
      color: #ffffff;
      font-size: 1.4rem;
    }

    .terms-and-conditions {
      color: #ffffff;
      font-size: 1.4rem;
      justify-self: center;
    }

    .social-media--icons {
      justify-self: end;

      .icon {
        &:not(:last-child) {
          margin-right: 2rem;
        }
      }
    }
  }
}
</style>
