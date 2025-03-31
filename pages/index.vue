<template>
  <section>
    <div class="relative w-full justify-center flex md:justify-start">
      <video class="z-1 w-full brightness-80 object-cover 
              max-md:min-h-screen md:h-auto md:max-h-[767px]" playsinline autoplay muted loop disablepictureinpicture
        nodownload nofullscreen noremoteplayback nopicture-in-picture poster="\video\mainscr.mp4"
        src="\video\mainscr.mp4">
      </video>
      <img class="absolute bottom-0 w-full z-2" src="\image\wave1.svg">
    </div>
  </section>
  <section>
    <div class="lg:px-[93.5px] px-[23.5px] mx-auto w-full lg:container flex pb-[28px] justify-end pt-[28px] md:pt-0">
      <h2 class="uppercase text-white font-title text-3xl md:text-5xl"  data-aos="fade-left" :data-aos-delay="200">новости</h2>
    </div>
    <div class="lg:px-[93.5px] px-[23.5px] mx-auto w-full lg:container flex pb-[28px] items-end space-x-[7px]">
      <p class="text-xl text-white">список последних новостей</p>
      <p class="text-s text-gray-300">все новости</p>
    </div>
    <div class=" xl:px-17.5 mx-auto w-full lg:container flex flex-wrap">
      <NewsCard v-for="n of 3" data-aos="fade-up"   :data-aos-delay="n * 200"/>
    </div>
    <div class="relative flex justify-center pt-[20px]">
      <img class="w-full" src="\image\wave2.svg">
      <div
        class="lg:px-[93.5px] px-[23.5px] mx-auto w-full lg:container flex pb-[10px] md:pb-[28px] xl:pb-[59px] justify-end pt-[28px] md:pt-0 absolute bottom-0">
        <h2 class="uppercase text-white font-title md:text-5xl text-3xl"  data-aos="fade-left" :data-aos-delay="200">Наши отзывы</h2>
      </div>
    </div>
  </section>
  <section class="overflow-hidden bg-[#C52B5D]/56 py-18">
    <div class="flex w-max animate-right space-x-5">
      <div class="review" v-for="n in 10" :key="'left-' + n">
        <Feedback name="Пользователь {{ n }}" rating="5" text="Отличное место! Рекомендую." />
      </div>

      <div class="review" v-for="n in 10" :key="'left-duplicate-' + n">
        <Feedback name="Пользователь {{ n }}" rating="5" text="Отличное место! Рекомендую." />
      </div>
    </div>

    <!-- Вторая строка (движется влево) -->
    <div class="flex w-max animate-left space-x-5 mt-5">
      <div class="review" v-for="n in 10" :key="'right-' + n">
        <Feedback name="Пользователь {{ n + 10 }}" rating="4" text="Хороший сервис, мне понравилось!" />
      </div>
      <div class="review" v-for="n in 10" :key="'right-duplicate-' + n">
        <Feedback name="Пользователь {{ n + 10 }}" rating="4" text="Хороший сервис, мне понравилось!" />
      </div>
    </div>

    <!-- Третья строка (движется вправо) -->
    <div class="flex w-max animate-right space-x-5 mt-5">
      <div class="review" v-for="n in 10" :key="'left2-' + n">
        <Feedback name="Пользователь {{ n + 20 }}" rating="5" text="Прекрасное место для отдыха!" />
      </div>
      <div class="review" v-for="n in 10" :key="'left2-duplicate-' + n">
        <Feedback name="Пользователь {{ n + 20 }}" rating="5" text="Прекрасное место для отдыха!" />
      </div>
    </div>
  </section>
  <img class="w-full" src="\image\wave (3).png">
  <div class="flex justify-center pt-2.5"><Button data-aos="fade-up"   :data-aos-delay="200" /></div>
  <section class="pt-[120px]">
    <div class="pb-[70px]">
      <NuxtLink to="/"><Shell data-aos="fade-right"   :data-aos-delay="200" title="АКЦИИ" description="Следите за акциями, чтобы не упустить выгодные предложения"
        image-url="/image/stocks.png" /></NuxtLink>
    </div>
    <div class="pb-[120px]">
    <NuxtLink to="/"><Shell data-aos="fade-right"   :data-aos-delay="200" title="ТУРНИРЫ" description="Учавствуйте в турнирах, занимайте призовые места и получайте вознаграждения"
      image-url="/image/tournament.png" /></NuxtLink></div>
  </section>
  <section class= "flex px-4 lg:px-17.5 mx-auto w-full lg:container">
    <div class="text-white  flex flex-col xl:max-w-[786px] pr-[6px] m:max-w-[60%]" data-aos="fade-right"   :data-aos-delay=" 200">
      <h2 class="uppercase text-3xl font-title md:text-5xl pb-[21px]" >о нас</h2>
      <p class="text-xl font-desc md:text-4xl"><span class="text-[#CB2754]">SHADOWPLAY</span> — это сеть современных компьютерных клубов, созданных для настоящих геймеров! Ультрасовременные PC, стильный дизайн, уютная атмосфера и дух киберспортивных побед — всё это ждёт вас в SHADOWPLAY. Здесь каждый найдёт идеальное место для игр, тренировок и незабываемого времени с друзьями!</p>
    </div>
    <div class="md:w-[100%] justify-center xl:block 2xl:flex hidden m:flex" data-aos="fade-down"   :data-aos-delay=" 200">
      <img  src="\image\pngwing.com (1).png">
    </div>
  </section>
  <div class="relative flex justify-center pt-[20px]">
      <img class="w-full" src="\image\waveOffer2.svg">
      <div
        class="lg:px-[93.5px] px-[23.5px] mx-auto w-full lg:container flex pb-[10px] md:pb-[28px] xl:pb-[59px] justify-end pt-[28px] md:pt-0 absolute bottom-0">
        <h2 class="uppercase text-white font-title md:text-5xl text-3xl" data-aos="fade-left" :data-aos-delay="200">Мы предлагаем</h2>
      </div>
    </div>
  <section class="min-h-[365px] bg-[#C52B5D]/56 flex justify-center items-center">
    <div class="xl:px-17.5 py-[28px]  mx-auto w-full lg:container flex flex-wrap space-y-10">
      <Offer colorCard="#9A55EF" desc="МОЩНОЕ И СОВРЕМЕННОЕ ОБОРУДОВАНИЕ" image-url="\image\Shadow.png" data-aos="fade-up" :data-aos-delay="1*200"/>
      <Offer colorCard="#6ACC70" desc="УДОБСТВО И КОМФОРТ" image-url="\image\comfort.png" data-aos="fade-up" :data-aos-delay="2*200"/>
      <Offer colorCard="#5595EF" desc="ТУРНИРЫ С ПРИЗОВЫМ ФОНДОМ, АКЦИИ И СПЕЦИАЛЬНЫЕ ПРЕДЛОЖЕНИЯ" image-url="\image\gift.png" data-aos="fade-up" :data-aos-delay="3*200"/>
    </div>
  </section>
  <div class="pb-[120px]">
  <img src="\image\waveOffer.svg" class="w-full"></div>
  <section class="flex justify-center items-center pb-[70px] px-4">
    <p class="text-white font-desc text-xl md:text-4xl uppercase text-center max-w-[1010px] " data-aos="fade-up" :data-aos-delay="200">В НАШИХ компьютерных клубах вы найдёте всё, что нужно для ярких эмоций и комфортного отдыха: ТОПОВЫЕ компьютеры, удобные игровые зоны и атмосферу, которая вдохновляет на победы, ДО ВСТРЕЧИ В <span class="text-[#CB2754]">SHADOWPLAY !</span></p>
  </section>
</template>
<script>
import AOS from 'aos';
import 'aos/dist/aos.css';
export default{
mounted() {
  AOS.init({
    duration: 1000,
    offset: 200, 
  });
},}
</script>