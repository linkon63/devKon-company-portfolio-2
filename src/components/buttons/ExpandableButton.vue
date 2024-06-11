<template>
  <div>
    <div class="group w-[166px] h-[52px] rounded-full flex justify-between items-center relative overflow-hidden cursor-pointer">
      <div class="pl-[12px] opacity-0 group-hover:opacity-100 transition ease-out duration-[.8s] scale-0 group-hover:scale-100 z-30">
        <span class="text-nowrap text-right text-white text-[20px]">View Details</span>
      </div>
      <div class="w-[52px] h-[52px] bg-[#0068dc] rounded-full flex justify-center items-center z-30">
        <a class="text-white"><img class="-rotate-[270deg] w-[23px] h-[24px]" src="../../assets/images/home/float_icon_small.png" /></a>
      </div>
      <div
        class="w-full h-full rounded-full bg-[#0068dc] absolute translate-x-full group-hover:translate-x-0 z-10 transition ease-out duration-[.8s]">

      </div>
    </div>
  </div>
</template>
<script setup>
import { defineProps, reactive } from "vue";

const props = defineProps(["bgColor"]);
</script>

<style scoped></style>
