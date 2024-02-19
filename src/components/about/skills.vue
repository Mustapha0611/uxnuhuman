<template>
  <div class="flex py-5 backdrop-blur-sm justify-center flex-col md:flex-row lg:ml-44 md:ml-10 mx-7 items-center md:items-start">
    <section class="flex-1 ">
      <h1 class="heading md:text-4xl md:text-left text-center text-2xl my-5 drop-shadow-xl text-gray-600 font-semibold">UX design <span class="heading dropshadow">Education</span></h1>
      <h2 class="mb-5 text-gray-600 drop-shadow-xl md:text-3xl heading font-semibold">Coursera</h2>
      <div class="flex items-center gap-3">
        <span>
          <img src="@/assets/GCC.png" alt="google cert" />
        </span>
        <section>
          <p  class="heading text-gray-700 font-semibold">Google UX Design Certification. NOV</p>
          <p  class="heading text-gray-700 font-semibold">2022</p>
        </section>
      </div>
      <h3  class="heading md:text-4xl my-5 drop-shadow-xl text-gray-600 md:text-left text-center text-2xl font-semibold">Experience</h3>
      <div>
        <article v-for="ex of exp" class="mb-5">
            <h4 class="heading md:text-2xl  mt-1 drop-shadow-xl text-gray-600 font-semibold">{{ ex.jobtitle }}</h4>
            <p class="mb-2 text-gray-600">{{ ex.duration }}</p>
        </article>
      </div>
    </section>
    <section class="flex-1 md:px-20">
        <h1 class="heading md:text-4xl text-2xl my-5 md:text-left text-center drop-shadow-md text-gray-600 font-semibold">Skills</h1>
        <h2 class="mb-5 text-gray-600 text-2xl drop-shadow-xl md:text-3xl heading font-semibold">General</h2>
        <div class="flex md:gap-5 gap-3 flex-wrap max-w-[23rem]">
            <span v-for="sk of skillSet" class="skill play">
                {{ sk.skill }}
            </span>
        </div>
    </section>
  </div>
</template>
<script setup>
import { ref } from "vue";

const exp = ref([
    {
        jobtitle:"Flower.live",
        duration:"Lead UI/UX Designer . Jan 2024- present"
    },
    {
        jobtitle:"Samplexample",
        duration:"Lead UI/UX Designer . Jul 2023- present"
    },
    {
        jobtitle:"InsideComputer",
        duration:"Graphics Designer . Dec 2022- present"
    },
    {
        jobtitle:"Popular Design Service",
        duration:"Graphics Designer . June 2020- Dec 2021"
    }, 
    {
        jobtitle:"NMAN Designs",
        duration:"UI/UX & Grapics Designer & Apr 2022- Jan 2023"
    },
]);
const skillSet = ref([
    {
      skill:'UI/UX'
    },
    {
        skill:"Wireframing"
    },
    {
      skill:"Storyboarding"
    },
    {
        skill:"Product Design"
    }, 
    {
      skill:"Usability testing"
    },
    {
        skill:"Design sprint"
    },
    {
        skill:"Branding"
    },
    {
        skill:"Web Design"
    },
    {
        skill:"Graphics Design"
    },
    {
        skill:"Animation"
    },
    {
        skill:"Microinteraction"
    },
    {
        skill:"User reseach"
    },
    {
        skill:"wireframing"
    }
]);
</script>
<style>
.skill {
  border-radius: 25px;
  padding: 5px 20px;
  
  color:rgb(255, 255, 255);
  background: linear-gradient(270deg, #ffb100 0.07%, #d45800 101.95%);
  box-shadow: 0px 0px 2px 2px rgba(0, 0, 0, 0.25);
}
.play {
  font-family: "Play", sans-serif;
}
</style>