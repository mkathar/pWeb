<template>
  <HeroSectionVue />
  <About />
  <Services />
  <Portfolio />
  <Prices />
  <Hireme />
  <Testmonial />
  <Blog />
  <Contact />
  <Footer />
</template>

<script>
import About from "../components/about.vue";
import HeroSectionVue from "../components/heroSection.vue";
import Services from "../components/services.vue";
import Portfolio from "../components/portfolio.vue";
import Prices from "../components/prices.vue";
import Hireme from "../components/hireMe.vue";
import Testmonial from "../components/testmonial.vue";
import Blog from "../components/blog.vue";
import Contact from "../components/contact.vue";
import Footer from "../components/footer.vue";
export default {
  data() {
    return {};
  },
  components: {
    HeroSectionVue,
    About,
    Services,
    Portfolio,
    Prices,
    Hireme,
    Testmonial,
    Blog,
    Contact,
    Footer,
  },
};
</script>
