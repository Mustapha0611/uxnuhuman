<template>
  <main>
    <h1
      class="text-center md:text-7xl text-5xl lg:text-7xl font-semibold heading"
    >
      About <span class="dropshadow">me</span>
    </h1>
    <div
      class="flex md:justify-center flex-col-reverse md:flex-row px-5 md:px-10 md:mt-10 my-5 md:pt-10 lg:px-24 lg:h-auto"
    >
      <div class="absolute left-3 top-0 hidden md:block">
        <img src="@/assets/elipse.png" alt="blur" />
      </div>
      <div
        class="absolute left-3 lg:top-[22rem] top-[45rem] md:top-[40rem] -z-10 lg:h-[45rem] md:h-[30rem] lg:w-[7rem] h-[30rem] w-[5rem]"
      >
        <img src="@/assets/left.png" alt="left" class="w-full h-full" />
      </div>
      <section class="flex-1 lg:ml-20 ">
        <article class="flex gap-4 items-baseline heading text-3xl font-semibold">
          <img src="@/assets/location.svg" alt="location" />
          Abuja, Nigeria
        </article>
        <p
          class="lg:max-w-[500px] pt-10 mb-10 text-[16px] md:text-[18px] backdrop-blur-sm bg-white/30 font-light"
        >
          Hello, I'm Nuhu, a seasoned UX designer with over 3 years of
          experience and a solid foundation in UI and graphics design.
        </p>

        <p
          class="lg:max-w-[600px] mb-10 text-[14px] md:text-[18px] backdrop-blur-sm bg-white/30 font-light"
        >
          I'm passionate about bringing accessibility to the digital interface
          and applying customer psychology for a more defined interaction to
          achieve the best.
        </p>
        <p
          class="lg:max-w-[600px] mb-10 text-[14px] md:text-[18px] backdrop-blur-sm bg-white/30 font-light"
        >
          My journey has equipped me with the skills to not just meet user needs
          but to anticipate and exceed them. Let's collaborate to transform
          ideas into seamless, user-friendly designs.
        </p>
        <p
          class="lg:max-w-[600px] mb-10 text-[14px] md:text-[18px] backdrop-blur-sm bg-white/30 font-light"
        >
          Beyond UX, my interests span the realm of technology—be it
          smartphones, PCs, cutting-edge gadgets, software, Blockchain, NFTs,
          and more. I have a BSc. in Biochemistry, funny right? Thats what
          passion can do. Additionally, I have a deep passion for reading books.
        </p>
      </section>
      <section
        class="flex flex-1 items-center  lg:min-w-[30rem] justify-center"
      >
        <div
          class="md:w-[20rem] md:h-[30rem] lg:w-[20rem] lg:h-[30rem] w-[15rem] h-[22rem] my-10 md:my-0"
        >
          <img src="@/assets/pp.png" alt="" class="w-full h-full" />
        </div>
        <div
          class="absolute right-0 lg:top-16 md:top-[10rem] top-[7rem] -z-20 md:w-[15rem] md:h-[40rem] lg:w-[25rem] lg:h-[55rem] w-[15rem] h-[30rem]"
        >
          <img
            src="@/assets/right.png"
            alt="right circle"
            class="h-full w-full"
          />
        </div>
      </section>
    </div>
    <div class="flex justify-center my-5">
      <section
        class="flex items-center my-5 flex-col md:flex-row justify-around w-[90%] h-[15rem] bg-white/30 backdrop-blur-md rounded-lg"
      >
        <article v-for="his in histories" class="flex items-center">
          <div>
            <img :src="his.img" alt="img" />
          </div>
          <div
            class="flex flex-col py-5 px-5 font-semibold text-[18px] lg:text-2xl"
          >
            <span>{{ his.time }}</span>
            <span>{{ his.Text }}</span>
          </div>
        </article>
      </section>
    </div>
  </main>
</template>
<script setup>
import { ref } from "vue";
import event from "@/assets/event.png";
import brief from "@/assets/briefcase1.png";
import connect from "@/assets/connect.png";

const histories = ref([
  {
    time: "3+",
    Text: "YEARS EXPERIENCE",
    img: event,
  },
  {
    time: "30+",
    Text: "PROJECT COMPLETED",
    img: brief,
  },
  {
    time: "10+",
    Text: "HAPPY CLIENT",
    img: connect,
  },
]);
</script>
<style scoped>
* {
  font-family: "Play", sans-serif;
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
.button-stlye {
  border-radius: 25px;
  padding: 0 20px;
  border: 3px solid #fff;
  background: linear-gradient(270deg, #ffb100 0.07%, #d45800 101.95%);
  box-shadow: 0px 0px 4.5px 2px rgba(0, 0, 0, 0.25);
}
.white {
  border-radius: 25px;
  border: 5px solid #d45800;
  padding: 0 20px;
  background: var(
    --www-aplussagency-com-1519199951171875-x-6775999755859375-default-nero,
    #fff
  );
  box-shadow: 0px 0px 18.1px 0px rgba(0, 0, 0, 0.25) inset;
}
</style>
