<template>
<header role="banner" class="flex justify-between items-center h-[10vh] bg-white px-4 md:px-10">
  <div class="">
    <router-link to="/" @click="menuToggle" @keyup.enter="menuToggle" >
      <img src="../assets/logo.svg" alt="Your Website Logo" class="w-32 h-16 md:h-16 md:w-44" />
    </router-link>
  </div>

  <nav role="navigation" class="flex md:justify-between">
    <ul role="menu" class="flex  items-center   gap-7 font-semibold text-[18px] flex-col md:flex-row absolute md:static md:h-auto bg-white w-full left-[-100%] h-[100dvh] transition-all top-0 justify-center"
        :class="{ show: showMenu }" >
      <span tabindex="0" @click="menuToggle"
            class="md:hidden absolute top-7 right-[5%] w-6 h-6 cursor-pointer opacity-0 transition-opacity"
            :class="{showContact : showMenu}">
            <img src="../assets/close.png" alt="Close" class="w-full h-full" />
      </span>
      <li role="menu item"><router-link to="/" @click="menuToggle">Home</router-link></li>
      <li role="menu item"><router-link to="/About" @click="menuToggle">About</router-link></li>
      <li role="menu item"><router-link to="/Portfolio" @click="menuToggle">Portfolio</router-link></li>
    </ul>
  </nav>

  <div class="absolute md:static md:h-auto md:w-auto w-full left-0 top-[30rem] md:top-0 flex items-end justify-center opacity-0 md:opacity-100 transition-opacity"
        :class="{showContact : showMenu}">
    <button aria-label="Contact" class="text-white md:px-7 md:py-3 linear py-2 px-5 rounded-md">Contact</button>
  </div>

  <button aria-label="Toggle Menu" aria-haspopup="true" class="md:hidden flex cursor-pointer" @click="menuToggle" @keyup.enter="menuToggle">
    <img src="../assets/hamburger.png" alt="Menu" class="w-8 h-8 aspect-square" />
  </button>
</header>

</template>
<script setup>
import { ref } from "vue";

const showMenu = ref(false);
const menuToggle = () => {
  showMenu.value = !showMenu.value;
  console.log(showMenu.value);
};
</script>
<style scoped>
.linear {
  background: linear-gradient(90deg, #ffb100 0.32%, #d45800 99.54%);
}
.router-link-exact-active {
  /* border-bottom: 2px solid #D45800; */
  color: #d45800;
}
.show {
  /* transform: translateX(100%); */
  left: 0;
  transition: 0.2s all;
}
.showContact{
  opacity:1;
  transition: opacity 1s linear;
}
</style>
