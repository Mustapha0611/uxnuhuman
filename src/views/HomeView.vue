<script setup>
  import hero from '../components/homee/hero.vue'
  import services from '@/components/homee/services.vue';
  import reviews from '@/components/homee/reviews.vue';
  import portfoliointro from '@/components/homee/portfoliointro.vue';
  import contact from '@/components/homee/contact.vue';
</script>

<template>
  <main>
    <hero />
    <services />
    <reviews />
    <portfoliointro />
    <contact />
  </main>
</template>
<style>
  .play{
 font-family: 'Nova Round', system-ui;
}
.inter{
    font-family: 'Inter', sans-serif;
}
</style>