<template>
    <div class="bg-black text-white pt-[9px] px-[15px] rounded-[20px] min-w-[361px] min-h-[95px]">

        <div class="flex items-center mb-2 space-x-[16px]">
            <p class=" font-medium text-s">Андрей С.</p>
            <div class="flex ">
                <span v-for="n in 5" :key="n" class="text-yellow-400 text-xl flex items-start"
                    :class="{ 'text-gray-600': n > 5 }">★</span>
            </div>
        </div>
        <p class="text-sm leading-relaxed">Хорошо провел время, отличное место!</p>
    </div>
</template>