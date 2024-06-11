<template>
  <section class="bg-[#FAFAFC]">
    <section class="container mx-auto px-6 sm:px-24 sm:py-8">
      <div class="">
        <div class="">
          <!-- heading section -->
          <div class="grid grid-cols-1 pt-10 sm:pt-[70px]">
            <div
              class="text-left font-r-semibold text-3xl sm:text-3xl md:text-4xl lg:text-[40px] text-[#6E6E73]">
              What we get?
            </div>
            <div
              class="text-left text-4xl sm:text-7xl md:text-8xl lg:text-[110px] font-r-b pt-6 font-r-b text-ellipsis text-[#212121]">
              Our Achievements
            </div>
            <p class="text-[#6E6E73] text-xl md:text-2xl pt-6 w-full md:w-9/12">
              Since our establishment, we have been delivering high-quality and
              sustainable software solutions for corporate purposes of worldwide
              businesses.
            </p>
          </div>

          <div class="lg:flex lg:justify-center pt-20 w-full">
            <swiper 
                :spaceBetween="30" 
                :effect="'fade'" 
                :modules="[Autoplay, Navigation]"
                :navigation="{ prevEl: '.prev', nextEl: '.next'}"
                class="mySwiper h-[100%] w-[100%] relative"
              >

              <swiper-slide class="">
                <div class="w-full grid grid-row lg:grid-cols-2 gap-8 lg:gap-4">
                  <div class="order-last lg:order-first max-w-[666px] max-h-[423px]">
                    <img class="h-full w-full"
                      src="../../../assets/images/home/achivment-section/achevement_image.png" />
                  </div>
                  <div class="flex flex-col justify-center lg:p-4">
                    <h2 class="capitalize text-3xl md:text-4xl lg:text-[48px] mb-[24px] font-r-b text-[#212121]">Mobile App Design</h2>
                    <p class="text-lg md:text-xl lg:text-[24px] text-[#212121] line-heigt-40">Lorem ipsum dolor sit, amet consectetur
                      adipisicing
                      elit. Iure quis alias dolorem est. Natus dolorem non corrupti ratione est rerum neque nisi eius.</p>
                  </div>
                </div>
              </swiper-slide>  
              

              <swiper-slide class="">
                <div class="w-full grid grid-row lg:grid-cols-2 gap-8 lg:gap-4">
                  <div class="order-last lg:order-first max-w-[666px] max-h-[423px]">
                    <img class="h-full w-full"
                      src="../../../assets/images/home/achivment-section/achevement_image.png" />
                  </div>
                  <div class="flex flex-col justify-center lg:p-4">
                    <h2 class="capitalize text-3xl md:text-4xl lg:text-[48px] mb-[24px] font-r-b text-[#212121]">Mobile App Design</h2>
                    <p class="text-lg md:text-xl lg:text-[24px] text-[#212121] line-heigt-40">Lorem ipsum dolor sit, amet consectetur
                      adipisicing
                      elit. Iure quis alias dolorem est. Natus dolorem non corrupti ratione est rerum neque nisi eius.</p>
                  </div>
                </div>
              </swiper-slide>                

              <div class="flex justify-center lg:justify-end w-full items-end">
                <div class="hidden md:block absolute md:flex z-20">
                <button
                  class="group w-[52px] h-[52px] rounded-full bg-[#9AC7FF] hover:bg-[#EEEEEE] flex justify-center items-center prev">
                  <span>
                    <img class="group-hover:hidden -rotate-[180deg]"
                      src="../../../assets//images/home/right_arrow_small.png" />
                    <img class="hidden group-hover:block" src="../../../assets//images/home/arrow_left_blue.png" />
                  </span>
                </button>
                <button
                  class="group w-[52px] h-[52px] rounded-full bg-[#0567E1] hover:bg-[#EEEEEE] flex justify-center items-center ml-[16px] next">
                  <img class="group-hover:hidden" src="../../../assets//images/home/right_arrow_small.png" />
                  <img class="hidden group-hover:block -rotate-[180deg]"
                    src="../../../assets//images/home/arrow_left_blue.png" />
                </button>
              </div>
              </div>

            </swiper>
          </div>
        </div>
      </div>
      <!-- faq section -->
      <div class="pt-[140px]">
        <div class="grid grid-cols-1 pt-6">
          <div
            class="text-left font-r-semibold text-2xl sm:text-3xl md:text-4xl lg:text-[40px] text-[#6E6E73]">
            Do you want to know more ?
          </div>
          <div
            class="text-left text-6xl sm:text-7xl md:text-8xl lg:text-[110px] font-semibold pt-6 font-r-b text-ellipsis">
            FAQ
          </div>
          <p class="text-[#6E6E73] text-base sm:text-lg md:text-xl lg:text-2xl pt-6 pb-[60px]">
            Since our establishment, we have been delivering high-quality and
            sustainable software solutions for corporate purposes of worldwide
            businesses.
          </p>
        </div>

        <div class="pb-28">
          <FaqSection id="accordion" heading="What makes Softzino diffrent from others software development companies"
            content="A Michigan based company approached us to develop a food delivery platform, which they would offer to local restaurants and delivery persons in a region as a third-party platform for getting the food to the doorstep of the customer. The customer would use the platform to find the nearest restaurants and get their food delivered to their destinations. A Michigan based company approached us to develop a food delivery platform, which they would offer to local restaurants and delivery persons in a region as a third-party platform for getting the food to the doorstep of the customer. The customer would use the platform to find the nearest restaurants and get their food delivered to their destinations." />
          <FaqSection id="accordion1" heading="How does Softzino ensure sustainablity of its software solution?"
            content=" Lorem Since our establishment, we have been delivering high-quality and
          sustainable software solutions for corporate purposes of worldwide
          businesses. Since our establishment, we have been delivering high-quality and
          sustainable software solutions for corporate purposes of worldwide
          businesses. ipsum, dolor sit amet consectetur adipisicing elit. Vero iure autem possimus ea saepe rerum praesentium? Neque ut labore harum culpa quia at nulla repudiandae!2lorem" />
          <FaqSection id="accordion2" heading="Can Softzino handle the entire software development lifecycle?"
            content=" Lorem Since our establishment, we have been delivering high-quality and
          sustainable software solutions for corporate purposes of worldwide
          businesses. Since our establishment, we have been delivering high-quality and
          sustainable software solutions for corporate purposes of worldwide
          businesses. ipsum, dolor sit amet consectetur adipisicing elit. Vero iure autem possimus ea saepe rerum praesentium? Neque ut labore harum culpa quia at nulla repudiandae!2lorem" />

          <FaqSection id="accordion3" heading="What industries does Softzino specialize in?"
            content=" Lorem Since our establishment, we have been delivering high-quality and
          sustainable software solutions for corporate purposes of worldwide
          businesses. Since our establishment, we have been delivering high-quality and
          sustainable software solutions for corporate purposes of worldwide
          businesses. ipsum, dolor sit amet consectetur adipisicing elit. Vero iure autem possimus ea saepe rerum praesentium? Neque ut labore harum culpa quia at nulla repudiandae!2lorem" />

          <FaqSection id="accordion4"
            heading="Does Softzino offer custom software solutions for startups and small businesses?"
            content=" Lorem Since our establishment, we have been delivering high-quality and
          sustainable software solutions for corporate purposes of worldwide
          businesses. Since our establishment, we have been delivering high-quality and
          sustainable software solutions for corporate purposes of worldwide
          businesses. ipsum, dolor sit amet consectetur adipisicing elit. Vero iure autem possimus ea saepe rerum praesentium? Neque ut labore harum culpa quia at nulla repudiandae!2lorem" />


        </div>
      </div>
    </section>
  </section>
</template>
<script setup>
import { reactive } from "vue";
import FaqSection from "../faq-section/FaqTab.vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay, Navigation, Pagination } from "swiper/modules";
const state = reactive({
  grayscaleLevelImg1: "grayscale",
  grayscaleLevelImg2: "grayscale",
  grayscaleLevelImg3: "grayscale",
  grayscaleLevelImg4: "grayscale",
  grayscaleLevelImg5: "grayscale",
});
</script>

<style scoped>
.line-heigt-40 {
  line-height: 40px;
}
</style>