<template>
  <div id="app">
    <app-header></app-header>
  </div>
</template>

<script>
import Header from './views/Header';

export default {
  components: {
    appHeader: Header
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
  font-family: 'Fira Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 1.6rem;
  font-weight: 300;
}
</style>
