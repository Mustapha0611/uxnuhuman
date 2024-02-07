<template>
  <div>
    <section>
      <h4 class="play font-semibold text-2xl text-center">GET IN TOUCH</h4>
      <P class="inter md:w-[50%] lg:w-[30%] mx-auto my-10 px-5">
        “ Feel free to send me a message, Lets have a chat and see how we can
        bring your idea to live ”
      </P>
    </section>
    <div class="flex justify-center pb-10">
      <section
        class="flex flex-col  lg:flex-row items-center rounded-se-[5rem] rounded-es-[5rem] play bg-gradient-to-l from-orange-400 to-orange-600 md:p-10 p-4 w-[94%] lg:w-[84%] pb-10 gap-5"
      >
        <div class="flex text-white xl:pl-20 justify-center flex-col md:w-1/2">
          <p class="lg:text-3xl md:text-2xl text-xl font-semibold mt-5">EMAIL: nuhualiyyu@gmail.com</p>
          <p class="lg:text-3xl md:text-2xl text-xl font-semibold my-5">PHONE: +23481 2062 8010</p>
          <article class="max-w-[28rem] h-64 hidden md:flex">
            <img src="@/assets/hands.png"  alt="shaking" class="w-full h-full" />
          </article>
        </div>
        <div class="flex md:w-1/2 justify-center items-center">
          <form action="">
            <div class="flex gap-3 mb-4 w-fit">
              <input
                type="text"
                name="Name"
                aria-label="Name"
                placeholder="Your Name"
                class="md:px-5 md:py-3 px-3 py-2 font-semibold rounded-lg w-[48%]"
              />
              <input
                type="text"
                name="Name"
                aria-label="Name"
                placeholder="Your Name"
                class="px-5 py-3 font-semibold rounded-lg w-[48%]"
              />
            </div>
            <div class="mb-4">
              <input
                type="email"
                name="email"
                aria-label="email"
                placeholder="Your Email"
                class="px-5 py-3 font-semibold w-full rounded-lg"
              />
            </div>
            <div>
              <textarea
                name="Message"
                aria-label="message"
                id=""
                cols="30"
                rows="6"
                class="w-full p-5 rounded-lg"
                placeholder="Your message"
              ></textarea>
            </div>
            <div>
              <button type="submit" 
              class="flex justify-center px-10 py-5 rounded-2xl bg-gray-200 font-semibold w-full"
              >Send Message</button>
            </div>
          </form>
        </div>
      </section>
    </div>
  </div>
</template>
<style scoped>
.play {
  font-family: "Nova Round", system-ui;
}
.inter {
  font-family: "Inter", sans-serif;
}
input, textarea{
  outline:none;
}
</style>
