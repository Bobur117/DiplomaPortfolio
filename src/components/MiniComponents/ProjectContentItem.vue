<template>
    <div class="slider">
        <swiper
            :slides-per-view="1"
            :space-between="25"
            :navigation="true"
            :modules="modules"
            :breakpoints="swiperOptions.breakpoints" 
            :pagination="{ clickable: true }"
            @slideChange="onSlideChange"
            class="myswiper"

            >
            <swiper-slide> <a href="https://bobur117.github.io/About-me/"><img src="../../assets/images/pr1.png" alt=""></a></swiper-slide>
            <swiper-slide> <a href="https://bobur117.github.io/Silver-house/"><img src="../../assets/images/pr2.png" alt=""></a></swiper-slide>
            <swiper-slide> <a href="https://bobur117.github.io/Gotrip/"><img src="../../assets/images/pr3.png" alt=""></a></swiper-slide>
            <swiper-slide> <a href="https://bobur117.github.io/Nike/"><img src="../../assets/images/pr4.png" alt=""></a></swiper-slide>
            <swiper-slide> <a href="https://bobur117.github.io/BoulevardMarket/"><img src="../../assets/images/pr5.png" alt=""></a></swiper-slide>
            <swiper-slide> <a href="https://bobur117.github.io/Grayson/"><img src="../../assets/images/pr6.png" alt=""></a></swiper-slide>
            <swiper-slide> <a href="https://bobur117.github.io/Vuecinema-Adaptive/"><img src="../../assets/images/pr7.png" alt=""></a></swiper-slide>
  
        </swiper>
    </div>
  
</template>

<script setup>
import { ref } from "vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation, Pagination, Scrollbar } from 'swiper/modules';
import 'swiper/css';
import 'swiper/css/navigation';
import 'swiper/css/pagination';

const modules = ref([Navigation]);

let swiperOptions = ref({
    breakpoints: {
        320: {
            slidesPerView: 1,
        },
        576: {
            slidesPerView: 1,
        },
        840:{
            slidesPerView: 1,
        },
        900: {
            slidesPerView: 2,
        },
        1200: {
            slidesPerView: 2,
        },
        1450: {
            slidesPerView: 2,
        },
    }
});




</script>

<style lang="scss">


.slider{
    margin-bottom: 50px;
    display: flex;
    justify-content: center;
    align-items: center;

    & img{
        width: 100%;
        height: 300px;
    }
}
.myswiper{
    width: 1000px;
}


</style>