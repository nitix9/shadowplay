<template>
  <NuxtRouteAnnouncer />
  <div class="bg-black">
    <header class="md:pt-[19px] fixed flex justify-center w-full z-100">
        <div
            class="flex bg-black/60 md:rounded-menu items-center w-full md:w-31/48 md:max-w-[930px] md:min-w-[755px]  md:min-h-[125px]">
            <nav class="flex justify-between md:justify-evenly w-full items-center py-3 px-4 md:py-0 md:px-0">
                <ul class="uppercase hidden  text-white md:flex justify-evenly items-center w-full">
                    <li>
                        <NuxtLink>о нас</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/news">новости</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink>цены</NuxtLink>
                    </li>
                </ul>
                <img src="\image\Logo.svg" class="hidden md:max-h-full md:flex ">
                <img src="\image\MobLogo.svg" class="flex md:hidden h-full">
                <p class="md:hidden">МоБ</p>
                <ul class="uppercase hidden text-white md:flex justify-evenly items-center w-full">
                    <li>
                        <NuxtLink>акции</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink>турниры</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink>вакансии</NuxtLink>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
    <NuxtPage />
    <footer class="md:pb-[15px]">
        <div class="bg-main md:footer-cont md:rounded-footer flex items-center flex-col md:w-[76.7%] md:max-w-[1104px] mx-auto">
        <div class="pt-[1rem] pb-[0.5rem] border-b-line/24 border-b-1 w-full md:max-w-[583px]">
            <ul class="uppercase text-white flex md:justify-evenly flex-wrap space-x-[10px] justify-center pr-[16px] pl-[16px] ">
                <li><NuxtLink>о нас</NuxtLink></li>
                <li><NuxtLink>новости</NuxtLink></li>
                <li><NuxtLink>цены</NuxtLink></li>
                <li><NuxtLink>акции</NuxtLink></li>
                <li><NuxtLink>турниры</NuxtLink></li>
                <li><NuxtLink>вакансии</NuxtLink></li>
            </ul>
        </div>
        <div class="pt-[1rem] pb-[1rem]">
            <ul class="uppercase text-white flex space-x-[0.6875rem]">
                <li><NuxtLink><img src="\image\LogoTg.svg"></NuxtLink></li>
                <li><NuxtLink><img src="\image\VK Logo (1).svg"></NuxtLink></li>
                <li><NuxtLink><img src="\image\whatsapp-color-svgrepo-com.png"></NuxtLink></li>
                <li><NuxtLink><img src="\image\Icon_RUTUBE_dark_color.png"></NuxtLink></li>
            </ul>
        </div>
        </div>
    </footer>
  </div>
</template>
