<template>
    <h1 class="heading md:text-3xl text-2xl my-5 drop-shadow-md text-gray-600 text-center font-semibold">Technical tools</h1>
    <div class="flex px-5 md:gap-12 gap-5 justify-center my-5">
        <span v-for="tool in tools" class="max-w-28 max-h-28">
            <img :src="tool.img" :alt="tool.alt" class="w-full h-full">
        </span>
    </div>
    <button class="flex items-center mx-auto my-20 md:w-2/3 lg:w-3/12 w-2/3  button-stlye">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="60"
              height="60"
              viewBox="0 0 60 60"
              fill="none"
            >
              <g clip-path="url(#clip0_144_252)">
                <mask
                  id="mask0_144_252"
                  style="mask-type: luminance"
                  maskUnits="userSpaceOnUse"
                  x="6"
                  y="0"
                  width="48"
                  height="60"
                >
                  <path
                    d="M53.6363 0.370117H6.18408V59.9701H53.6363V0.370117Z"
                    fill="white"
                  />
                </mask>
                <g mask="url(#mask0_144_252)">
                  <g opacity="0.605491">
                    <path
                      d="M29.9735 22.9531C33.9913 22.9531 37.2534 26.2153 37.2534 30.233C37.2534 34.2508 33.9913 37.513 29.9735 37.513C25.9557 37.513 22.6936 34.2508 22.6936 30.233C22.6936 26.2153 25.9557 22.9531 29.9735 22.9531Z"
                      fill="#0ECB3D"
                      fill-opacity="0.50196"
                    />
                  </g>
                  <g opacity="0.395491">
                    <path
                      d="M29.9735 18.707C36.3348 18.707 41.4997 23.8719 41.4997 30.2333C41.4997 36.5946 36.3348 41.7595 29.9735 41.7595C23.6122 41.7595 18.4473 36.5946 18.4473 30.2333C18.4473 23.8719 23.6122 18.707 29.9735 18.707Z"
                      fill="#0ECB3D"
                      fill-opacity="0.50196"
                    />
                  </g>
                  <g opacity="0.185491">
                    <path
                      d="M29.9735 14.4609C38.6783 14.4609 45.746 21.5286 45.746 30.2335C45.746 38.9383 38.6783 46.006 29.9735 46.006C21.2686 46.006 14.2009 38.9383 14.2009 30.2335C14.2009 21.5286 21.2686 14.4609 29.9735 14.4609Z"
                      fill="#0ECB3D"
                      fill-opacity="0.50196"
                    />
                  </g>
                  <path
                    d="M29.9734 24.377C33.2058 24.377 35.8303 27.0014 35.8303 30.2339C35.8303 33.4663 33.2058 36.0908 29.9734 36.0908C26.7409 36.0908 24.1165 33.4663 24.1165 30.2339C24.1165 27.0014 26.7409 24.377 29.9734 24.377Z"
                    fill="#0ECB3D"
                  />
                </g>
              </g>
              <defs>
                <clipPath id="clip0_144_252">
                  <rect
                    width="59.6"
                    height="59.6"
                    fill="white"
                    transform="translate(0.110107 0.370117)"
                  />
                </clipPath>
              </defs>
            </svg>
            <span class="text-white md:text-base text-sm"> Download Resume </span>
          </button>
</template>
<script setup>
import { ref } from 'vue';
import Ai from '@/assets/Ai.png';
import figma from '@/assets/figma.png';
import ps from '@/assets/ps.png';
import diamond from '@/assets/diamond.png';
import xd from '@/assets/xd.png';

 const tools = ref([
    {
        img:figma,
        alt:"figma"
    },
    {
        img:xd,
        alt:"Adobe Xd"
    },
    {
        img:Ai,
        alt:"Adobe illustrator"
    },
    {
        img:ps,
        alt:"Adobe Photoshop"
    },
    {
        img:diamond,
        alt:"diamond"
    },
 ])
</script>
<style scoped>
.button-stlye {
  border-radius: 25px;
  padding: 0 20px;
  border: 3px solid #fff;
  background: linear-gradient(270deg, #ffb100 0.07%, #d45800 101.95%);
  box-shadow: 0px 0px 4.5px 2px rgba(0, 0, 0, 0.25);
}
</style>