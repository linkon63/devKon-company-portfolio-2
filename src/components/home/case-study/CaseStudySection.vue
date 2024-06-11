<template>
  <section class="bg-[#FAFAFC] pb-20 lg:pb-[140px]">
    <section class="container mx-auto px-6 sm:px-24">
      <section class="pt-32 lg:pt-[140px]" id="ourservices">
        <div class="">
          <div
            class="text-center font-r-semibold text-xl md:text-2xl lg:text-3xl xl:text-[40px] text-[#6E6E73]"
          >
            Our Strength
          </div>
          <div
            class="text-center text-5xl sm:text-6xl md:text-7xl lg:text-[84px] font-r-b pt-6"
          >
            Case Study
          </div>
          <p
            class="text-center text-2xl text-[#6E6E73] pt-10 px-6 md:px-12 lg:px-24 xl:px-48"
          >
            Since our establishment, we have been delivering high-quality and
            sustainable software solutions for corporate purposes of worldwide
            businesses.
          </p>
        </div>

        <div class="pt-10 md:pt-20">
          <div class="grid grid-col-1 lg:grid-cols-2 gap-8">
            <div class="p-2 sm:p-6 rounded-3xl bg-white ">
              <div class="">
                <img
                  class="w-full"
                  src="../../../assets//images/home/case-study/cs1.png"
                />
              </div>
              <div class="px-3 pt-12">
                <h2 class="font-r-semibold text-3xl lg:text-[32px]">
                  Industry Expertise & Experience
                </h2>
                <p class="text-2xl leading-10 pt-[32px]">
                  Lorem Ipsum is simply dummy text of the printing and
                  typesetting industry. Lorem Ipsum has been the industry.
                </p>
              </div>

              <div class="w-[100%] flex justify-end pt-[32px]">
                <ExpandButton />
              </div>
            </div>
            <div class="p-2 sm:p-6 rounded-3xl bg-white ">
              <div class="">
                <img
                  class="w-full"
                  src="../../../assets//images/home/case-study/cs3.png"
                />
              </div>
              <div class="px-3 pt-12">
                <h2 class="font-r-semibold text-3xl lg:text-[32px]">
                  Industry Expertise & Experience
                </h2>
                <p class="text-2xl leading-10 pt-[32px]">
                  Lorem Ipsum is simply dummy text of the printing and
                  typesetting industry. Lorem Ipsum has been the industry.
                </p>
              </div>

              <div class="w-[100%] flex justify-end pt-[32px]">
                <ExpandButton />
              </div>
            </div>
          </div>
        </div>
      </section>
    </section>
  </section>
</template>
<script setup>
import ExpandButton from "../../buttons/ExpandableButton.vue";
</script>
