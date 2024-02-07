<template>
    <div class="xl:px-36 lg:px-20 md:px-10 px-5 play py-10">
        <section class="flex justify-between">
        <h2  class="font-semibold text-3xl ">
            Portfolio
        </h2>
        <button type="button" class="flex md:w-52 px-5 h-14 text-white rounded-md items-center justify-center gap-6 bg-gradient-to-r from-orange-400 to-orange-600">
           <span> View All</span>
           <img src="@/assets/arrow.png" alt="arrow right" class="w-12 h-12" />
        </button>
        </section>
        <section class="mb-10">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-4 mt-20">
                <article class="border-2 border-orange-300 flex items-center flex-col justify-center py-10 rounded-lg">
                    <div class="flex justify-between">
                        <img src="@/assets/1.png" class="md:h-64 md:max-w-40 min-w-10 hover:translate-y-8 transition-all hover:scale-110" alt="phone"><img src="@/assets/2.png" class="md:h-64 md:max-w-40 min-w-10 hover:translate-y-8 transition-all hover:scale-110" alt="secondphone"><img src="@/assets/3.png" class="md:h-64 md:max-w-40 min-w-10 hover:translate-y-8 transition-all hover:scale-110" alt="thirdphone">
                    </div>
                    <h3 class="font-semibold text-center text-xl md:text-2xl mt-10">
                        Aquasmart Mobile app design
                    </h3>
                </article>
                <article class="border-2 border-orange-300 flex items-center flex-col justify-center py-10 rounded-lg">
                    <div class="flex justify-between px-3">
                        <img src="@/assets/4.png" class="md:h-64 md:max-w-36 min-w-5 hover:translate-y-8 transition-all hover:scale-110" alt="phone"><img src="@/assets/5.png" class="md:h-64 md:max-w-36 min-w-5 hover:translate-y-8 transition-all hover:scale-110" alt="secondphone"><img src="@/assets/6.png" class="md:h-64 md:max-w-36 min-w-5 hover:translate-y-8 transition-all hover:scale-110" alt="thirdphone">
                    </div>
                    <h3 class="font-semibold text-xl md:text-2xl px-2 text-center  mt-10">
                        Collection connection app design
                    </h3>
                </article>
            </div>
            <div class="grid grid-cols-1 my-5 relative ">
                <article class="border-2 border-orange-300 py-10  rounded-lg px-5">
                    <div class="flex justify-evenly items-end ">
                        <img src="@/assets/rect.png" class="md:h-64 h-20  md:max-w-40 min-w-10 left-10  hover:translate-y-8 transition-all hover:scale-110" alt="phone"><img src="@/assets/lap.png" class="md:h-88 md:max-w-[40rem] min-w-[10rem] hover:translate-y-8 transition-all hover:scale-110" alt="secondphone"><img src="@/assets/tab.png" class="md:h-72 h-20 min-w-15 md:max-w-48 hover:translate-y-8 transition-all hover:scale-110" alt="thirdphone">
                    </div>
                    <h3 class="font-semibold text-xl md:text-2xl mt-10 text-center">
                        Webite Design For p2p peace plan
                    </h3>
                </article>
            </div>
        </section>
   
    </div>
</template>
<!-- <style scoped>
.play{
 font-family: 'Nova Round', system-ui;
}
.inter{
    font-family: 'Inter', sans-serif;
}
</style> -->