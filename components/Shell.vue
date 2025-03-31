<template>
  <div class="px-4">
    <div
      class="relative mx-auto  flex bg-[#FF0052]/3 text-white rounded-lg shadow-[4px_4px_4px_0_rgba(197,43,93,0.8)] max-w-[1053px] border-[#C52B5D]/56 border-1 overflow-hidden group">
      <div
        class="absolute z-[-1] inset-0 bg-[#C52B5D]/20 translate-x-[-100%] group-hover:translate-x-0 transition-transform duration-1000 ease-in-out"
      ></div>
      <div class="flex-1 md:pt-[27px] md:pl-[56px] px-4 py-4 ">
        <h2 class="font-regular pb-[14px] text-2xl md:text-5xl">{{ title }}</h2>
        <p class="leading-relaxed font-desc text-xl md:text-4xl md:max-w-[539px]">
          {{ description }}
        </p>
      </div>
      <div class="py-[26px] md:pr-[20px] lg:pr-[53px] md:pl-[34px] pr-2 items-center xs:flex hidden">
        <div
          class="flex-shrink-0 rounded-[20px] bg-cover bg-no-repeat bg-center w-[150px] h-[160px] md:w-[300px] md:h-[200px] xl:w-[371px] xl:h-[254px]"
          :style="{ backgroundImage: 'url(' + imageUrl + ')' }">
        </div>
      </div>
    </div>
  </div>
</template>
<script>

export default {
  props:{
    title: {
      type: String,
      default: 'Default Title'
    },
    description: {
      type: String,
      default: 'Default Description'
    },
    imageUrl: {
      type: String,
      default: '/image/stocks.png'
    },
    link:{type:String, default:'/'},
  }
}
</script>