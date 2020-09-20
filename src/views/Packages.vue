<template>
  <div id="packages" class="packages-container">
    <app-package-header></app-package-header>
    <app-package-content></app-package-content>
  </div>
</template>

<script>
import PackagesHeader from '../components/PackagesHeader';
import PackagesContent from '../components/PackageContent';

export default {
  components: {
    appPackageHeader: PackagesHeader,
    appPackageContent: PackagesContent
  }
};
</script>

<style lang="scss">
.packages-container {
  margin: 5rem 10rem 8rem;

  @media screen and (max-width: 1024px) {
    margin: 5rem 1rem 8rem;
  }

  @media screen and (max-width: 768px) {
    margin: 5rem;
  }

  @media screen and (max-width: 425px) {
    margin: 5rem 1rem;
  }
}
</style>
