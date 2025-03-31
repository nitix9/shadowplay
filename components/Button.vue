<template>
<NuxtLink
        :to="link"
        class="relative group px-6 py-3 text-white bg-[#1A1A2E] rounded-lg overflow-hidden shadow-[4px_4px_10px_0_rgba(197,43,93,0.8)] min-w-[207px] inline-flex items-center justify-center"
    >
        <span
            class="absolute inset-0 bg-[#C52B5D] transition-transform duration-300 ease-in transform translate-x-full group-hover:translate-x-0"
        ></span>
        <span class="relative z-10 transition-transform duration-300 group-hover:translate-x-1 font-desc">
            {{ label }}
        </span>
    </NuxtLink>
</template>
<script>
export default {
    props: {
        label: {
            type: String,
            default: "ВСЕ ОТЗЫВЫ",
        },
        link:{
            type: String,
            default: "/",
        }
    },
};
</script>