<template>
  <div id="about" class="header-container">
    <app-navbar :scroll-value="this.scrollValue"></app-navbar>
    <header class="header-section">
      <app-jumbotron></app-jumbotron>
    </header>
  </div>
</template>

<script>
import Navbar from '../components/Navbar';
import Jumbotron from '../components/Jumbotron';

export default {
  props: ['scrollValue'],
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
    clip-path: ellipse(70% 80% at 50% 20%);

    @media screen and (max-width: 768px) {
      background-size: cover;
      // clip-path: circle(68.5% at 50% 20%);
    }
  }
}
</style>
