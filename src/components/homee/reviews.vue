<template>
    <main class="w-full flex justify-center my-20 ">
        <div class="w-[90%] h-auto my-5">
            <h2 class="play mb-5 font-semibold text-3xl p-10">Reviews</h2>
            <Splide :options="options"  aria-label="Reviews">
                <SplideSlide v-for="review of reviews" class="" >
                    <section class="flex justify-between items-center italic ">
                       <span class="font-semibold">{{ review.name }}</span> <img :src="review.img" alt="service images">
                    </section>
                    <!-- <h3 class="text-center font-semibold text-2xl play">{{ review.title }}</h3> -->
                    <p class="inter py-5 px-10">{{ review.text }}</p>
                </SplideSlide>
            </Splide>
        </div>
    </main>
 
</template>
<script setup>
import { ref } from "vue"
import us from "@/assets/us.png"
import ger from "@/assets/ger.png"
import est from "@/assets/est.png"
import '@splidejs/splide/css'
// import '@splidejs/vue-splide/css/skyblue';
// import '@splidejs/vue-splide/css/sea-green';

    const options={
        // hasTrack:false,
        type: 'loop',
        rewind: true,
        gap:'5rem',
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
    const reviews = ref([
        {
            img: us,
            name:"Marc Egeth",
            text:"“ Nuhu is a creative and talented designer. You can see his work publicly posted at sampleXample.com  ...........”"
        },
        {
            img: est,
            name:'Till Carlos',
            text:"“ He did great work on my App Mockups. 5/5 would hire again”"
        },
        {
            img: ger,
            name:'Daniel Becker',
            text:"“ Fast and fluent communication and work. Did even more mockups than”"
        }
    ])
</script>
<style scoped>
.play{
 font-family: 'Nova Round', system-ui;
}
.inter{
    font-family: 'Inter', sans-serif;
}
</style>