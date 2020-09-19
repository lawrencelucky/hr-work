<template>
  <div class="header-container">
    <header class="header-section">
      <app-navbar></app-navbar>
      <app-jumbotron></app-jumbotron>
    </header>
  </div>
</template>

<script>
import Navbar from '../components/Navbar';
import Jumbotron from '../components/Jumbotron';

export default {
  components: {
    appNavbar: Navbar,
    appJumbotron: Jumbotron
  }
};
</script>

<style lang="scss">
.header-container {
  color: #ffffff;

  .header-section {
    background-image: linear-gradient(
        0.08deg,
        rgba(0, 0, 0, 0) 15.36%,
        rgba(0, 0, 0, 0.688) 90.13%
      ),
      url(../assets/images/header.png);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: top;
  }
}
</style>
