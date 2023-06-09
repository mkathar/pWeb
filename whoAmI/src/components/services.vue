<template>
  <div class="service">
    <span class="service__ques">What I Do ?</span>
    <h1 class="service__title">Service</h1>
    <div class="service__group">
      <div class="service__group__item">
        <div class="service__group__item__content">
          <Icon
            class="service__group__item__content__icon"
            name="responsive"
            :size="55"
          />
          <span class="service__group__item__content__text">Responsive</span>
        </div>
        <div class="service__group__item__content__hide">
          <p class="service__group__item__content__hide__text">
            responsive tasarımlar yapabiliyorum
          </p>
        </div>
      </div>
      <div class="service__group__item">
        <div class="service__group__item__content">
          <Icon
            class="service__group__item__content__icon"
            name="pencilCase"
            :size="55"
          />
          <span class="service__group__item__content__text">Design</span>
        </div>
        <div class="service__group__item__content__hide">
          <p class="service__group__item__content__hide__text">
            dizayn tasarımlar yapabiliyorum
          </p>
        </div>
      </div>
      <div class="service__group__item">
        <div class="service__group__item__content">
          <Icon
            class="service__group__item__content__icon"
            name="analytics"
            :size="55"
          />
          <span class="service__group__item__content__text">Statistics</span>
        </div>
        <div class="service__group__item__content__hide">
          <p class="service__group__item__content__hide__text">
            Statistics bunu da yaparım
          </p>
        </div>
      </div>
      <div class="service__group__item">
        <div class="service__group__item__content">
          <Icon
            class="service__group__item__content__icon"
            name="toolbox"
            :size="55"
          />
          <span class="service__group__item__content__text">Techs</span>
        </div>
        <div class="service__group__item__content__hide">
          <p class="service__group__item__content__hide__text">
            Alet Çantam da var
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import { Icon } from "../icons.jsx";
</script>
<script>
export default {
  data() {
    return {};
  },
};
</script>
