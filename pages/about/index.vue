<template>
  <div class="wrapper-content wrapper-content--fixed">
    <img class="about-image" src="@/assets/images/bikes_1.jpeg" alt="bikes" />
    <!-- <h1 class="about-title">About my blog</h1> -->
    <section class="about">
      <div class="container">
        <Intro :title="title"/>
      </div>
    </section>
  </div>
</template>

<script>
import Intro from "@/components/UI/Intro.vue";
export default {
  components: { Intro },
  data() {
    return {
        title: 'About my blog'
    }
  }
};
</script>

<style lang="scss" scoped>
.wrapper-content.wrapper-content--fixed {
  margin-top: 60px;
}
.about-image {
  position: relative;
}
</style>
