<template>
<section class="relative w-full min-h-screen md:min-h-[60vh]">
    <div class="w-full">
        <div class="block">
            <video class="absolute z-[-1] top-0 left-0 w-full brightness-80 object-cover 
                  min-h-screen md:h-auto md:max-h-[767px] md:min-h-[60vh]" 
                  playsinline autoplay muted loop disablepictureinpicture nodownload nofullscreen noremoteplayback nopicture-in-picture 
                  poster="..\..\video\mainscr.mp4" src="..\..\video\mainscr.mp4">
            </video>
        </div>
        <div class="pl-[16px] pr-[16px] absolute top-0 items-start md:items-stretch pt-[215px] max-md:pt-[100px] md:pl-[12%] md:pr-[12%] md:block md:h-auto bg-blur-2xl overflow-hidden w-full">
            <div class="  uppercase md:max-w-[810px]">
                <h1 class="text-3xl md:max-lg:text-4xl lg:text-5xl text-white animate-slideInOut">Проведи время в нашем компьютерном клубе с мощным железом</h1>
            </div>
        </div>
    </div>
    <div class="absolute bottom-0 w-full flex justify-end">
        <img src="..\..\image\wave1.svg">
    </div>
</section>
</template>