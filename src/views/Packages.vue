<template>
  <div class="packages-container">
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
  margin: 5rem 10rem;
}
</style>
