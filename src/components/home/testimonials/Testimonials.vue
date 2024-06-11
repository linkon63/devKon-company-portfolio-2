<template>
  <div class="w-full bg-[#fff] relative pb-12">
    <section
      class="container mx-auto px-7 sm:px-16 md:px-20 lg:px-24 mt-4"
    >
      <section class="bg-white pb-14 xl:pb-16 2xl:pb-20">
        <div class="text-center">
          <!-- heading section -->
          <p
            class="pb-6 pt-16 lg:pt-20 xl:pt-[110px] text-2xl md:text-3xl lg:text-4xl xl:text-[40px] text-[#6E6E73] font-r-semibold"
          >
            Testimonials
          </p>
          <div class="py-2">
            <h1
              class="text-[#212121] text-4xl sm:text-5xl md:text-6xl lg:text-7xl xl:text-8xl 2xl:text-[110px] font-r-b capitalize"
            >
              What client
            </h1>
            <h1
              class="text-[#212121] text-4xl sm:text-5xl md:text-6xl lg:text-7xl xl:text-8xl 2xl:text-[110px] font-r-b capitalize"
            >
              Says About us
            </h1>
          </div>
        </div>
      </section>
    </section>
    <!-- slider section -->
    <!-- carasoul -->
    
    <TestimonialsSlider />
  </div>
</template>

<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import ExpandableButton from "../../buttons/ExpandableButton.vue";
import TestimonialsSlider from "./TestimonialsSlider.vue";
import "@dotlottie/player-component";
// Import Swiper styles
import "swiper/css";

import "swiper/css/effect-coverflow";
import "swiper/css/pagination";

// import required modules
import { EffectCoverflow, Pagination, Autoplay } from "swiper/modules";
import TestimonialsSliderVue from "./TestimonialsSlider.vue";
</script>

<style scoped>
.swiper {
  width: 100%;
  padding-top: 50px;
  padding-bottom: 50px;
}

.swiper-slide {
  background-position: center;
  background-size: cover;
  width: 300px;
  /* height: 550px; */
}

.swiper-slide img {
  display: block;
  width: 100%;
}

.swiper-slide-visible > .mainDiv > p {
  display: none;
}

.swiper-slide-prev > .mainDiv > .expandableBtnShow {
  display: none;
  border: 2px solid green;
}

.swiper-slide-next > .mainDiv > .expandableBtnShow {
  border: 2px solid yellow;
  display: none;
}
</style>
