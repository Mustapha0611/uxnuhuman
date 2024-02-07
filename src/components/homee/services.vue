<template>
    <main class="w-full flex justify-center ">
        <div class="w-[86%] h-auto my-5">
            <h2 class="play mb-5 font-semibold text-3xl">SERVICES I PROVIDE</h2>
            <Splide :options="options"  aria-label="Services">
                <SplideSlide v-for="service of services" class="border-2 border-orange-400 rounded-xl">
                    <section class="flex justify-center items-center h-[13rem]">
                        <img :src="service.img" alt="service images">
                    </section>
                    <h3 class="text-center font-semibold text-2xl play">{{ service.title }}</h3>
                    <p class="inter p-5">{{ service.text }}</p>
                </SplideSlide>
            </Splide>
        </div>
    </main>
 
</template>
<script setup>
import { ref } from "vue"
import present from "@/assets/presentation.png"
import design from "@/assets/design.png"
import monitor from "@/assets/monitor.png"
import '@splidejs/splide/css'
// import '@splidejs/vue-splide/css/skyblue';
// import '@splidejs/vue-splide/css/sea-green';

    const options={
        // hasTrack:false,
        type: 'loop',
        rewind: true,
        gap:'1rem',
        perPage: 3,
        breakpoints: {
            1020: {
            perPage: 2,
            },
          640: {
            perPage: 1,
            },
        }
    }
    const services = ref([
        {
            img: present,
            title:"UI/UX DESIGNER",
            text:"“ Elevating digital experiences through intuitive design and seamless user interactions. ”"
        },
        {
            img: design,
            title:"APP & WEBSITE DESIGN",
            text:"“ Get your unique, professional website live in less than a week, With CMS, flexibility and full control. ”"
        },
        {
            img: monitor,
            title:"GRAPHIC DESIGN",
            text:"“Transforming concepts into visually compelling narratives through creative and impactful graphic design.”"
        }
    ])
</script>
<!-- <style scoped>
.play{
 font-family: 'Nova Round', system-ui;
}
.inter{
    font-family: 'Inter', sans-serif;
}
</style> -->