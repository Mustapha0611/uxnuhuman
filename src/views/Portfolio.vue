<template>
    <main>
        <div class="flex justify-center gap-10 font-semibold play">
            <router-link :to="{name:'ui'}">UI/UX Design</router-link>
            <router-link :to="{name:'graphics'}">Graphic Design</router-link>
        </div>
        <Transition name="fade">
          <RouterView  />
         </Transition>
    </main>
</template>
<script setup>
    import { RouterView } from 'vue-router';
</script>
<style scoped>
.router-link-exact-active {
    color: #d45800;
}
.play{
 font-family: 'Nova Round', system-ui;
}
.inter{
    font-family: 'Inter', sans-serif;
}
</style>