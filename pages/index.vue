<template>
    <section>
    <div class="relative w-full justify-center flex md:justify-start">
        <video class="z-1 w-full brightness-80 object-cover 
              max-md:min-h-screen md:h-auto md:max-h-[767px]" playsinline autoplay muted loop disablepictureinpicture nodownload nofullscreen noremoteplayback nopicture-in-picture poster="..\video\mainscr.mp4" src="..\video\mainscr.mp4">
        </video>
        <img class="absolute bottom-0 w-full z-2" src="..\image\wave1.svg"> 
    </div>
    </section>
    <section>
        <div class="lg:px-[93.5px] px-[23.5px] mx-auto w-full lg:container flex pb-[28px] justify-end pt-[28px] md:pt-0">
            <h2 class="uppercase text-white font-title text-5xl">новости</h2>
        </div>
        <div class="lg:px-[93.5px] px-[23.5px] mx-auto w-full lg:container flex pb-[28px] items-end space-x-[7px]">
            <p class="text-xl text-white">список последних новостей</p>
            <p class="text-s text-gray-300">все новости</p>
        </div>
        <div class=" lg:px-17.5 mx-auto w-full lg:container flex flex-wrap">
        <NewsCard v-for="n of 3"/>
        </div>
        <img class="w-full" src="..\image\wave (2).svg">

    </section>
    <br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
</template>