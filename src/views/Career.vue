<template>
  <div class="career-container">
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
}
</style>
