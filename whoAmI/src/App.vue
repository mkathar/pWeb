<template>
  <RouterView />
</template>

<script>
import { RouterView } from "vue-router";
import Home from "./pages/Home.vue";
export default {
  data() {
    return {};
  },
  components: {
    Home,
    RouterView,
  },
};
</script>
