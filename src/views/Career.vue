<template>
  <div id="careers" class="career-container">
    <app-career-header></app-career-header>
    <app-career-content></app-career-content>
  </div>
</template>

<script>
import CareerHeader from '../components/CareerHeader';
import CareerContent from '../components/CareerContent';

export default {
  components: {
    appCareerHeader: CareerHeader,
    appCareerContent: CareerContent
  }
};
</script>

<style lang="scss">
.career-container {
  padding: 7rem 14rem;

  @media screen and (max-width: 1024px) {
    padding: 7rem 1rem;
  }

  @media screen and (max-width: 768px) {
    padding: 5rem;
  }

  @media screen and (max-width: 425px) {
    padding: 5rem 1rem;
  }
}
</style>
