<template>
  <div class="blog-container">
    <app-blog-header></app-blog-header>
    <app-blog-content></app-blog-content>
  </div>
</template>

<script>
import BlogHeader from '../components/BlogHeader';
import BlogContent from '../components/BlogContent';

export default {
  components: {
    appBlogHeader: BlogHeader,
    appBlogContent: BlogContent
  }
};
</script>

<style lang="scss">
.blog-container {
  padding: 7rem 14rem;
  background-image: linear-gradient(
      0.8deg,
      rgba(0, 33, 71, 0.5),
      rgba(0, 33, 71, 0.5)
    ),
    url(../assets/images/blog.png);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: top;
}
</style>
