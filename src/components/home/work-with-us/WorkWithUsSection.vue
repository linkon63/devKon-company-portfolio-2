<template>
  <section id="ourworks" class="bg-[#FAFAFC]">
    <section class="w-full flex justify-center container mx-auto px-6 sm:px-24">
      <div class="flex justify-center pb-12">
        <div class="">
          <!-- heading section -->
          <div class="">
            <div class="text-center pt-16 md:pt-20 lg:pt-24 xl:pt-28">
              <h1
                class="text-[#212121] text-4xl sm:text-6xl md:text-7xl lg:text-8xl xl:text-[110px]capitalize font-r-b"
              >
                Who Worked &
              </h1>
              <h1
                class="text-[#212121] text-4xl sm:text-6xl md:text-7xl lg:text-8xl xl:text-[110px] font-semibold sm:pt-6 font-r-b text-ellipsis"
              >
                Working With Us
              </h1>
            </div>

            <div class="flex justify-center">
              <p
                class="pt-8 text-xl md:text-2xl w-5/6 text-left sm:text-center text-[#6E6E73] leading-8"
              >
                Since our establishment, we have been delivering high-quality
                and sustainable software solutions for corporate purposes of
                worldwide businesses.
              </p>
            </div>

            <div class="w-full pt-12 lg:pt-20 flex justify-center">
              <!-- top section -->
              <div
                class="grid grid-cols-1 md:grid-cols-1 lg:grid-cols-3 gap-8"
              >
                <!-- box 1 -->
                <div class="max-w-[420px] flex justify-center">
                  <Card 
                    logo = "apple_icon2.png"
                    title = "Apple"
                    description = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit quisquam."
                    hoverTitle = "Apple"
                    hoverDescription = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit quisquam."
                  />
                </div>
                <!-- box2 -->

                <div class="max-w-[420px] flex justify-center">
                  <Card 
                    logo = "arbys_1.png"
                    title = "Arbys"
                    description = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit quisquam."
                    hoverTitle = "Arbys"
                    hoverDescription = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit quisquam."
                  />
                </div>
                <!-- box3 -->

                <div class="max-w-[420px] flex justify-center">
                  <Card 
                    logo = "redis_1.png"
                    title = "Redis"
                    description = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit quisquam."
                    hoverTitle = "Redis"
                    hoverDescription = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit quisquam."
                  />
                </div>
              </div>
            </div>
            <!-- down section -->
            <div class="w-full pt-12 flex justify-center">
              <div
                class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-8"
              >
                <!-- box 1 -->
                <div class="max-w-[420px] flex justify-center">
                  <Card 
                    logo = "godaddy_2.png"
                    title = "GoDaddy"
                    description = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit quisquam."
                    hoverTitle = "GoDaddy"
                    hoverDescription = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit quisquam."
                  />
                </div>
                <!-- box2 -->
                <div class="max-w-[420px] flex justify-center">
                  <Card 
                    logo = "fiirefox_1.png"
                    title = "Firefox"
                    description = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit quisquam."
                    hoverTitle = "Firefox"
                    hoverDescription = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit quisquam."
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </section>
</template>


<script setup>
  import Card from './Card.vue';


</script>

