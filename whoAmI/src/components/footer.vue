<template>
  <footer class="footer">
    <p class="footer__copyright">KATHAR</p>
    <div class="footer__group">
      <span class="footer__group__ıcon"
        ><Icon name="twitter" :size="32"
      /></span>
      <span class="footer__group__ıcon"
        ><Icon name="linkedin" :size="32"
      /></span>
      <span class="footer__group__ıcon"><Icon name="github" :size="32" /></span>
    </div>
  </footer>
</template>

<script>
import { Icon } from "../icons.jsx";
export default {
  data() {
    return;
  },
  components: { Icon },
};
</script>
