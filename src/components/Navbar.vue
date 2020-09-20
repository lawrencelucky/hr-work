<template>
  <div class="navbar-container">
    <div :class="this.scrollValue === true ? 'scroll' : ''" class="navbar">
      <div class="navbar-brand">
        <a href="#"
          ><img
            v-if="!this.scrollValue"
            src="../assets/icons/hr-work-logo.svg"
            alt="hr-work-logo"
            class="navbar-brand--logo"/>
          <img
            v-if="this.scrollValue"
            src="../assets/icons/hr-work-logo-dark.svg"
            alt="hr-work-logo"
            class="navbar-brand--logo"
        /></a>
      </div>
      <nav>
        <ul>
          <li class="nav-list">
            <a class="nav-link" href="#whoweare">Who we are</a>
          </li>
          <li class="nav-list">
            <a class="nav-link" href="#packages">Packages</a>
          </li>
          <li class="nav-list"><a class="nav-link" href="#blog">Blog</a></li>
          <li class="nav-list">
            <a class="nav-link" href="#careers">Careers</a>
          </li>
          <li class="nav-list">
            <a class="nav-link" href="#contact">Contact</a>
          </li>
        </ul>
      </nav>
      <div class="toggler-container">
        <div class="toggler-icon">
          <img src="../assets/icons/menu.svg" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['scrollValue']
};
</script>

<style lang="scss">
.navbar-container {
  .navbar {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1000000;
    padding: 3rem 12rem;
    display: flex;
    justify-content: space-between;
    transition: all 0.5s;

    @media screen and (max-width: 1024px) {
      padding: 3rem 7rem;
    }

    @media screen and (max-width: 768px) {
      padding: 3rem 5rem;
    }

    @media screen and (max-width: 425px) {
      padding: 2rem 1rem;
    }

    .navbar-brand {
      img {
        @media screen and (max-width: 1024px) {
          width: 80%;
        }

        @media screen and (max-width: 425px) {
          width: 60%;
        }
      }
    }

    nav {
      @media screen and (max-width: 768px) {
        display: none;
      }

      ul {
        display: flex;
        align-items: center;

        .nav-list {
          list-style: none;

          &:not(:last-child) {
            margin-right: 4rem;
          }

          .nav-link {
            text-decoration: none;
            color: #ffffff;
            font-weight: 600;
            transition: all 0.5s;

            &:hover {
              color: #ef0633;
            }
          }
        }
      }
    }
  }

  .scroll {
    background-color: #ffffff;
    transition: all 0.5s;
    padding: 2rem 8rem;

    @media screen and (max-width: 1024px) {
      padding: 2rem 5rem;
    }

    @media screen and (max-width: 768px) {
      padding: 2rem 4rem;
    }

    @media screen and (max-width: 425px) {
      padding: 1rem;
    }

    nav {
      display: flex;
      align-items: center;

      @media screen and (max-width: 768px) {
        display: none;
      }

      ul {
        .nav-list {
          .nav-link {
            color: #ef0633;
            transition: all 0.3s;
          }
        }
      }
    }
  }

  .toggler-container {
    display: none;
    align-items: center;

    .toggler-icon {
      img {
        width: 3rem;

        @media screen and (max-width: 425px) {
          width: 2rem;
        }
      }
    }

    @media screen and (max-width: 768px) {
      display: flex;
    }
  }
}
</style>
