<template>
  <swiper
    :spaceBetween="30"
    :centeredSlides="true"
    :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"
    :pagination="{
      clickable: true,
    }"
    :navigation="true"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide><img src="./../assets/1 (1).jpg" /></swiper-slide>
    <swiper-slide><img src="./../assets/1 (2).jpg" /></swiper-slide>
    <swiper-slide><img src="./../assets/1 (3).jpg" /></swiper-slide>
    <swiper-slide><img src="./../assets/1 (1).jpg" /></swiper-slide>
    <swiper-slide><img src="./../assets/1 (2).jpg" /></swiper-slide>
    <swiper-slide><img src="./../assets/1 (3).jpg" /></swiper-slide>
  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

import "./../style.css";

// import required modules
import { Autoplay, Pagination, Navigation } from "swiper";

export default {
  name: "CarosuelView",
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
    };
  },
};
</script>
