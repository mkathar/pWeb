<template>
  <header
    :class="{ 'header--unpinned': scrolled }"
    v-on="handleScroll"
    class="header"
  >
    <h1 class="header__title">KATHAR</h1>
    <ul class="header__list">
      <li class="header__list--item">Home</li>
      <li class="header__list--item">About</li>
      <li class="header__list--item">Portfolio</li>
      <li class="header__list--item">Testmonial</li>
      <li class="header__list--item">Blog</li>
      <li class="header__list--item">Contact</li>
      <li class="header__list--item">
        <label for="ChangeTheme">
          <input
            @change="dark"
            v-model="checked"
            type="checkbox"
            id="ChangeTheme"
          />
          <span class="slide"></span>
        </label>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  data() {
    return {
      checked: null,
      limitPosition: 500,
      scrolled: false,
      lastPosition: 0,
    };
  },
  methods: {
    handleScroll() {
      if (
        this.lastPosition < window.scrollY &&
        this.limitPosition < window.scrollY
      ) {
        this.scrolled = true;
      }

      if (this.lastPosition > window.scrollY) {
        this.scrolled = false;
      }

      this.lastPosition = window.scrollY;
    },
    dark() {
      if (this.checked == true) {
        console.log(this.checked);
        document.body.classList.toggle("dark");
        const hero = document.querySelector(".hero");
        hero.classList = "dark-hero";
      } else {
        console.log(this.checked);
        document.body.classList = "";
        const hero = document.querySelector(".dark-hero");
        hero.classList = "hero";
      }
    },
  },
  created() {
    window.addEventListener("scroll", this.handleScroll);
  },
  destroyed() {
    window.removeEventListener("scroll", this.handleScroll);
  },
};
</script>

<style lng="scss"></style>
