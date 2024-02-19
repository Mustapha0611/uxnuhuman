<template>
  <main>
    <h1
      class="text-center md:text-7xl text-5xl lg:text-7xl font-semibold drop-shadow-xl heading"
    >
      About <span class="dropshadow">me</span>
    </h1>
    <div
      class="flex md:justify-center flex-col-reverse md:flex-row px-5 md:px-10 md:mt-10 my-5 md:pt-10 lg:px-24 lg:h-auto"
    >
      <div class="absolute left-[35rem] top-[27rem] hidden md:block">
        <img src="@/assets/elipse.png" alt="blur" />
      </div>
      <div
        class="absolute left-3 lg:top-[22rem] top-[45rem] md:top-[40rem] -z-10 lg:h-[45rem] md:h-[30rem] lg:w-[7rem] h-[30rem] w-[5rem]"
      >
        <img src="@/assets/left.png" alt="left" class="w-full h-full" />
      </div>
      <section class="flex-1 lg:ml-20 backdrop-blur-sm bg-white/30">
        <article class="flex gap-4 items-baseline heading text-3xl font-semibold">
          <img src="@/assets/location.svg" alt="location" />
          Abuja, Nigeria
        </article>
      
        <p
          class="lg:max-w-[500px] pt-10 mb-5 text-[14px] md:text-[16px] play font-light"
        >
          Hello, I'm Nuhu, a seasoned UX designer with over 3 years of
          experience and a solid foundation in UI and graphics design.
        </p>

        <p
          class="lg:max-w-[600px] mb-5 text-[14px] md:text-[16px] play font-light"
        >
          I'm passionate about bringing accessibility to the digital interface
          and applying customer psychology for a more defined interaction to
          achieve the best.
        </p>
        <p
          class="lg:max-w-[600px] mb-5 text-[14px] md:text-[16px] play font-light"
        >
          My journey has equipped me with the skills to not just meet user needs
          but to anticipate and exceed them. Let's collaborate to transform
          ideas into seamless, user-friendly designs.
        </p>
        <p
          class="lg:max-w-[600px] mb-5 text-[14px] md:text-[16px] play font-light"
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
          class="absolute right-0 lg:top-16 md:top-[10rem] top-[7rem] -z-20 md:w-[15rem] md:h-[40rem] lg:w-[25rem] lg:h-[45rem] w-[15rem] h-[30rem]"
        >
          <img
            src="@/assets/right.png"
            alt="right circle"
            class="h-full w-full"
          />
        </div>
      </section>
    </div>
  </main>
</template>

<style>
.play {
  font-family: "Play", sans-serif;
}

</style>
