<template>
  <div class="header-container">
    <header class="header-section">
      <app-navbar></app-navbar>
    </header>
  </div>
</template>

<script>
import Navbar from '../components/Navbar';

export default {
  components: {
    appNavbar: Navbar
  }
};
</script>

<style lang="scss">
.header-container {
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
    height: 100vh;
  }
}
</style>
