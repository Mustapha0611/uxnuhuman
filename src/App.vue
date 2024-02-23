<script setup>
// import { AOS } from 'aos';
import { RouterView } from 'vue-router'
import headerSection from './components/headerSection.vue';
import footerSection from '@/components/footerSection.vue';

</script>

<template>
  <div class="bg-gradient-to-r from-primary to-secondary h-auto">
    <headerSection  class="sticky top-0 z-40"/>
    <Transition name="fade">
      <RouterView class="-z-40" />
    </Transition>
    <footerSection /> 
  </div>
</template>

<style>

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
.heading {
  font-family: "Nova Round", system-ui;
}

.dropshadow {
  background: linear-gradient(90deg, #ffb100 36.42%, #d45800 94.44%);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  /* font-size: 76px; */
  font-style: normal;
  /* font-weight: 700; */
  line-height: normal;
  text-decoration-line: underline;
  border-bottom: #d45800 solid 4px;
}
</style>