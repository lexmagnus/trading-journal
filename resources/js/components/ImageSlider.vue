<script setup lang="ts">
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Navigation, Pagination, Autoplay } from 'swiper/modules';

import 'swiper/css';
import 'swiper/css/navigation';
import 'swiper/css/pagination';

const images = [
    '/img/slider1.jpg',
    '/img/slider2.jpg',
    '/img/slider3.jpg',
    '/img/slider4.jpg'
];
</script>

<style scoped>
.mySwiper {
    width: 100vw;
    height: 90vh;
}
</style>

<template>
    <Swiper :modules="[Navigation, Pagination, Autoplay]" navigation pagination :autoplay="{
        delay: 3000,
        disableOnInteraction: false
    }" loop class="mySwiper">
        <SwiperSlide v-for="(img, i) in images" :key="i">
            <img :src="img" class="w-full h-auto object-cover rounded-lg shadow-md" />
        </SwiperSlide>
    </Swiper>
</template>