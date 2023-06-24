<template>
  <header
    :class="{ 'header--unpinned': scrolled }"
    v-on="handleScroll"
    class="header"
  >
    <div class="header__group">
      <h1 class="header__group__title">KATHAR</h1>
      <ul class="header__group__list">
        <li class="header__group__list--item">Home</li>
        <li class="header__group__list--item">About</li>
        <li class="header__group__list--item">Portfolio</li>
        <li class="header__group__list--item">Testmonial</li>
        <li class="header__group__list--item">Blog</li>
        <li class="header__group__list--item">Contact</li>
      </ul>
    </div>
    <label class="header__theme" for="ChangeTheme">
      <input
        @change="dark"
        v-model="checked"
        type="checkbox"
        id="ChangeTheme"
      />
      <span class="slide"></span>
    </label>
    <div class="header__menuToggle">
      <input type="checkbox" />

      <span></span>
      <span></span>
      <span></span>

      <ul class="header__menu">
        <a href="#"><li>Home</li></a>
        <a href="#"><li>About</li></a>
        <a href="#"><li>Portfolio</li></a>
        <a href="#"><li>Blog</li></a>
        <a href="#"><li>Contact</li></a>
        <label class="header__theme__hamburger" for="ChangeTheme">
          <input
            @change="dark"
            v-model="checked"
            type="checkbox"
            id="ChangeTheme"
          />
          <span class="slide"></span>
        </label>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      checked: false,
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
        const title = document.querySelector(".header__group__title");
        title.style.color = "#1e549f";
        const list = document.querySelector(".header__group__list");
        list.style.color = "#1e549f";
      }

      if (this.lastPosition > window.scrollY) {
        this.scrolled = false;
        const title = document.querySelector(".header__group__title");
        title.style.color = "#fff";
        const list = document.querySelector(".header__group__list");
        list.style.color = "#fff";
      }

      if (this.lastPosition > 500 && this.checked == false) {
        const title = document.querySelector(".header__group__title");
        title.style.color = "#1e549f";
        const list = document.querySelector(".header__group__list");
        list.style.color = "#1e549f";
      } else {
        const title = document.querySelector(".header__group__title");
        title.style.color = "#fff";
        const list = document.querySelector(".header__group__list");
        list.style.color = "#fff";
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
