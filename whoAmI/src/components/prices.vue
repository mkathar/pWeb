<template>
  <div class="prices">
    <span class="prices__ques">How Much I Charge ?</span>
    <h1 class="prices__title">My Pricing</h1>
    <div class="prices__group">
      <div class="prices__group__content">
        <h1 class="prices__group__content__title">Free</h1>
        <Icon name="scooter" :size="70" />
        <span class="prices__group__content__item">Selam</span>
        <span class="prices__group__content__item">Selam</span>
        <span class="prices__group__content__item">Selam</span>
        <span><Icon name="x" :size="16" /></span>
        <span><Icon name="x" :size="16" /></span>
        <span><Icon name="x" :size="16" /></span>
        <span class="prices__group__content__price"></span>
        <button class="prices__group__content__button btn-tertiary">
          Subscribe
        </button>
      </div>
      <div class="prices__group__content">
        <h1 class="prices__group__content__title">Basic</h1>
        <Icon name="shipped" :size="70" />
        <span class="prices__group__content__item">Selam</span>
        <span class="prices__group__content__item">Selam</span>
        <span class="prices__group__content__item">Selam</span>
        <span><Icon name="x" :size="16" /></span>
        <span><Icon name="x" :size="16" /></span>
        <span><Icon name="x" :size="16" /></span>
        <span class="prices__group__content__price"></span>
        <button class="prices__group__content__button btn-tertiary">
          Subscribe
        </button>
      </div>
      <div class="prices__group__content">
        <h1 class="prices__group__content__title">Premium</h1>
        <Icon name="startup" :size="70" />
        <span class="prices__group__content__item">Selam</span>
        <span class="prices__group__content__item">Selam</span>
        <span class="prices__group__content__item">Selam</span>
        <span><Icon name="x" :size="16" /></span>
        <span><Icon name="x" :size="16" /></span>
        <span><Icon name="x" :size="16" /></span>
        <span class="prices__group__content__price"></span>
        <button class="prices__group__content__button btn-tertiary">
          Subscribe
        </button>
      </div>
    </div>
  </div>
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
