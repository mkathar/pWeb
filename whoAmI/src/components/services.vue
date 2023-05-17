<template>
  <div class="service">
    <span class="service__ques">What I Do ?</span>
    <h1 class="service__title">Service</h1>
    <div class="service__group">
      <div class="service__group__item">
        <Icon name="responsive" :size="55" />
        <span class="service__group__item__text">Responsive</span>
      </div>
      <div class="service__group__item">
        <Icon name="toolbox" :size="55" />
        <span class="service__group__item__text">Techs</span>
      </div>
      <div class="service__group__item">
        <Icon name="analytics" :size="55" />
        <span class="service__group__item__text"> Bişey yok</span>
      </div>
      <div class="service__group__item">
        <Icon name="pencilCase" :size="55" />
        <span class="service__group__item__text">Design</span>
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

console.log(Icon);
</script>
