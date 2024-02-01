<template>
  <div>
    <section>
      <h4 class="play font-semibold text-2xl text-center">GET IN TOUCH</h4>
      <P class="inter md:w-[30%] mx-auto my-10">
        “ Feel free to send me a message, Lets have a chat and see how we can
        bring your idea to live ”
      </P>
    </section>
    <section class="flex bg-gradient-to-l from-orange-400 to-orange-600 mx-20">
      <div class="flex-1 flex items-center justify-center flex-col">
        <p>EMAIL: nuhualiyyu@gmail.com</p>
        <p>PHONE: +23481 2062 8010</p>
        <article>
          <img src="@/assets/hands.png" alt="" />
        </article>
      </div>
      <div class="flex-1 flex items-center">
        <form action="">
          <div class="flex gap-3 mb-4">
            <input
              type="text"
              name="Name"
              aria-label="Name"
              placeholder="Your Name"
              class="px-5 py-3 font-semibold rounded-lg"                                 
            />
            <input
              type="text"
              name="Name"
              aria-label="Name"
              placeholder="Your Name"
              class="px-5 py-3 font-semibold rounded-lg"
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
              rows="10"
              class="w-full"
            ></textarea>
          </div>
          <div>
            <button type="submit">Send Message</button>
          </div>
        </form>
      </div>
    </section>
  </div>
</template>
