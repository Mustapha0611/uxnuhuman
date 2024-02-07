<template>
    <div class="flex w-[96%] mx-auto border-2 items-center justify-evenly h-52 my-10 rounded-xl play flex-col">
        <section>
            <ul class="flex items-center">
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url" target="_blank"><img :src="link.img" class="w-15 h-15" :alt="link.alt"></a>
                </li>
            </ul>
        </section>
        <section class="font-semibold text-xl">
            &copy; 2023 NUHU ALIYU
        </section>
    </div>
</template>
<script setup>
import { ref } from 'vue';
import behance from '@/assets/behance.png'
import dribble from '@/assets/dribble.png'
import linkedin from '@/assets/linkedin.png'
import ig from '@/assets/ig.png'
    const links = ref([
        {
            url:'',
            img:dribble,
            alt:"dribble"
        },
        {
            url:'',
            img:behance,
            alt:"behance"
        },
        {
            url:'',
            img:linkedin,
            alt:"linkedin"
        },
        {
            url:'',
            img:ig,
            alt:"ig"
        }
    ])
</script>