<template>
    <div class="flex w-[96%] mx-auto border-2 items-center justify-evenly h-52 my-10 rounded-xl play flex-col">
        <section>
            <ul class="flex items-center gap-5">
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url" target="_blank"><img :src="link.img" class="w-15 h-15" :alt="link.alt"></a>
                </li>
            </ul>
        </section>
        <section class="font-semibold text-xl play text-center">
            <p class="text-3xl py-3">nuhualiyyu@gmail.com</p>
            &copy; 2023 NUHU ALIYU
        </section>
    </div>
</template>
<script setup>
import { ref } from 'vue';
import twitter from '@/assets/twitter.png'
import dribble from '@/assets/dribble.png'
import linkedin from '@/assets/linkedin.png'
import ig from '@/assets/ig.png'
    const links = ref([
        {
            url:'https://www.dribbble.com/nuhuman',
            img:dribble,
            alt:"dribble"
        },
        {
            url:'https://twitter.com/Nuhuman01?t=A-1xs0soRxAkf7KZWbCQFw&s=09',
            img:twitter,
            alt:"twitter"
        },
        {
            url:'https://www.linkedin.com/in/nuhu-aliyu-18b37b234?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app',
            img:linkedin,
            alt:"linkedin"
        },
        {
            url:'https://www.instagram.com/nuhumaan?utm_source=qr&igsh=YzU1NGVlODEzOA%3D%3D',
            img:ig,
            alt:"ig"
        }
    ])
</script>