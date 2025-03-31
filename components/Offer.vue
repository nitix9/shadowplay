<template>
    <div class="px-[23.5px] md:px-[15px] lg:px-[23.5px] md:w-[33.3%] w-full">
        <div class="  h-[220px] rounded-menu flex items-center justify-evenly bg-[url(/image/Shadow.png)]"
            :style="{ background: colorCard }">
            <img :src="imageUrl" class="md:w-[33%] hidden 2xs:flex pr-[6px]">
            <div class="flex justify-center">
            <p class="uppercase text-white font-desc max-w-[200px]">{{ desc }}</p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        colorCard: {
            type: String,
            default: '#FF0052'
        },
        desc: {
            type: String,
            default: 'Киберспортивные турниры'
        },
        imageUrl: {
            type: String,
            default: '/image/Shadow.png'
        },
    },
}
</script>