<template>
  <div class="who-we-are-container">
    <div class="who-we-are-section">
      <app-whoweareheader></app-whoweareheader>
      <app-whowearecontent></app-whowearecontent>
    </div>
  </div>
</template>

<script>
import Whoweareheader from '../components/WhoWeAreHeader';
import Whowearecontent from '../components/WhoWeAreContent';

export default {
  components: {
    appWhoweareheader: Whoweareheader,
    appWhowearecontent: Whowearecontent
  }
};
</script>

<style lang="scss">
.who-we-are-container {
  margin: 5rem 10rem;
}
</style>
