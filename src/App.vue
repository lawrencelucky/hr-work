<template>
  <div id="app">
    <app-header :scroll-value="this.scroll"></app-header>
    <app-whoweare></app-whoweare>
    <app-packages></app-packages>
    <app-blog></app-blog>
    <app-career></app-career>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './views/Header';
import Whoweare from './views/WhoWeAre';
import Packages from './views/Packages';
import Blog from './views/Blog';
import Career from './views/Career';
import Footer from './views/Footer';

export default {
  data() {
    return {
      scroll: false
    };
  },
  created() {
    window.addEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      if (window.scrollY <= 0) {
        this.scroll = false;
      } else {
        this.scroll = true;
      }
    }
  },
  components: {
    appHeader: Header,
    appWhoweare: Whoweare,
    appPackages: Packages,
    appBlog: Blog,
    appCareer: Career,
    appFooter: Footer
  }
};
</script>

<style lang="scss">
*,
*::after,
*::before {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
}

#app {
  font-family: 'Source Sans Pro', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 1.6rem;
  font-weight: 300;
  letter-spacing: 0.9px;

  @media screen and (max-width: 425px) {
    font-size: 1.3rem;
  }
}
</style>
