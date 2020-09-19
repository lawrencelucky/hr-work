<template>
  <div class="navbar-container">
    <div class="navbar">
      <div class="navbar-brand">
        <a href="#"
          ><img
            src="../assets/icons/hr-work-logo.svg"
            alt="hr-work-logo"
            class="navbar-brand--logo"
        /></a>
      </div>
      <nav>
        <ul>
          <li class="nav-list">
            <a class="nav-link" href="#">Who we are</a>
          </li>
          <li class="nav-list"><a class="nav-link" href="#">Packages</a></li>
          <li class="nav-list"><a class="nav-link" href="#">Blog</a></li>
          <li class="nav-list"><a class="nav-link" href="#">Careers</a></li>
          <li class="nav-list"><a class="nav-link" href="#">Contact</a></li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.navbar-container {
  .navbar {
    padding: 4rem 12rem;
    display: flex;
    justify-content: space-between;

    nav {
      ul {
        display: flex;

        .nav-list {
          list-style: none;

          &:not(:last-child) {
            margin-right: 4rem;
          }

          .nav-link {
            text-decoration: none;
            color: #ffffff;
            font-weight: 600;
            transition: all 0.3s;

            &:hover {
              color: #ffffffc8;
            }
          }
        }
      }
    }
  }
}
</style>
