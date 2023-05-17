<template>
  <HeroSectionVue />
  <About />
  <Services />
  <Portfolio />
  <Prices />
</template>

<script>
import About from "./components/about.vue";
import HeroSectionVue from "./components/heroSection.vue";
import Services from "./components/services.vue";
import Portfolio from "./components/portfolio.vue";
import Prices from "./components/prices.vue";

export default {
  data() {
    return {};
  },
  components: { HeroSectionVue, About, Services, Portfolio, Prices },
};
</script>
