<template>
  <section id="ourcompany" class="pb-[80px] bg-[#fff] mt-[140px] mb-[60px]">
    <div class="container mx-auto flex justify-center">
      <div class="grid grid-cols-1">
        <div class="flex justify-center">
          <div class="px-8">
            <!-- heading section -->
            <div
              class="text-center graydeep font-r-semibold text-2xl sm:text-3xl md:text-4xl lg:text-[40px] text-[#6E6E73] mb-[22px] mt-[80px]">
              Where are we?
            </div>
            <div class="text-[#212121] text-center text-5xl sm:text-6xl md:text-7xl lg:text-[84px] font-r-b">
              Our Clients
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container mx-auto bg-white-700 background-map flex justify-center mt-[60px]">
      <div class="max-w-[1220px] max-h-[610px]">
        <div class="world-map">
          <img src="../../../assets/images/home/Map_new.png" alt="World Map" />

          <div class="absolute h-[10px] w-[10px] md:h-[15px] md:w-[15px] lg:h-[20px] lg:w-[20px] rounded-full usa">
            <span class="relative flex h-full w-full">
              <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-[#4D9CFF] opacity-75"></span>
              <span class="relative inline-flex rounded-full h-full w-full bg-sky-500"></span>
            </span>
          </div>
          <div @click="showLocation('bangladesh_location')" class="absolute h-[5px] w-[5px] rounded-full bangladesh cursor-pointer">
            <span class="relative flex h-full w-full">
              <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-[#4D9CFF] opacity-75"></span>
              <span class="relative inline-flex rounded-full h-full w-full bg-sky-500"></span>
            </span>
          </div>
          <div class="absolute h-[10px] w-[10px] md:h-[15px] md:w-[15px] lg:h-[20px] lg:w-[20px] rounded-full japan">
            <span class="relative flex h-full w-full">
              <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-[#4D9CFF] opacity-75"></span>
              <span class="relative inline-flex rounded-full h-full w-full bg-sky-500"></span>
            </span>
          </div>
          <div id="bangladesh_location" class="absolute hidden top-[20%] left-[39%]">
            <Location
              id="bangladesh_location"
              liveMap="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d58387.15328335826!2d90.31873084856971!3d23.847134507184272!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3755c41087fd55d5%3A0x1342e9e70c75ff57!2sSoftzino%20Technologies!5e0!3m2!1sen!2sbd!4v1716725710800!5m2!1sen!2sbd"
              title="Bangladesh Office" address="Tropical Akhand Tower, 23 Gareeb-e-Nawaz Ave, Dhaka 1230"
              phone="+8812345678" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import Location from './shared/Location.vue';
const showLocation = (id) => {
  let element = document.getElementById(id);
  if (element.classList.contains("hidden")) {
    element.classList.remove("hidden");
  } else {
    element.classList.add("hidden");
  }
};
</script>

<style scoped>
.world-map {
  width: 100%;
  position: relative;
}

.world-map img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.usa {
  top: 39%;
  left: 19%;
}

.japan {
  top: 77.4%;
  left: 83.3%;
}

.bangladesh {
  top: 50.8%;
  left: 71.5%;
}
</style>