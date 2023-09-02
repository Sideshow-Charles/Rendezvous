<template>
  <div class="landing__page">
    <!-- Landing page hero section -->
    <div class="hero__section">
      <!-- <div class="header__container"> -->
        <Header></Header>
      <!-- </div> -->

    </div>
  </div>
</template>

<script>
import Header from "../components/UI/header.vue"
export default {
  components: {
    Header,
  }
}
</script>
<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.hero__section {
  background-image: url("../assets/hero-image.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-color: lightgray 50%;
  height: 640px;
}

/* .header__container {
  margin: 50px 64px;
} */
</style>