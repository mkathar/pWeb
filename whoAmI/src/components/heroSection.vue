<template>
  <Header />
  <div class="hero">
    <span class="hero__up">HI!</span>
    <span class="hero__mid">I am Muhammed</span>
    <span class="hero__mid">KATAR</span>

    <span class="hero__bot">JR FRONTEND DEVELOPER</span>
    <button class="hero__btn btn-primary">Visit My Works</button>
  </div>
</template>

<script>
import Header from "./header.vue";

export default {
  data() {
    return {};
  },
  components: { Header },
};
</script>
