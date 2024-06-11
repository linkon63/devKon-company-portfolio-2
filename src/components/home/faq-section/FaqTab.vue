<template>
  <div
    class="border-s-0 border-b-[1px] py-4 cursor-pointer"
    @click="onShow"
    :id="id"
  >
    <div class="flex">
      <h3
        class="w-10/12 text-xl sm:text-2xl md:text-3xl lg:text-[32px] font-r-semibold"
      >
        {{
          heading
            ? heading
            : "What makes Softzino diffrent from others software development companies"
        }}
      </h3>
      <div class="w-2/12 flex justify-end items-center">
        <div
          :class="
            state.rotation
              ? 'transition duration-500 ease-in rotate-0'
              : 'transition duration-500 ease-in rotate-0'
          "
        >
          
        <img v-if="state.rotation" src="../../../assets/images/home/achivment-section/plus_icon.png" />
        <img v-else src="../../../assets/images/home/achivment-section/minus_icon.png" />

        </div>
      </div>
    </div>
  </div>
  <div class="panel cursor-wait">
    <div class="py-4 text-lg md:text-xl lg:text-2xl">
      <span class="text-[#212121] leading-10">
        {{ content ? content : "lorem" }}
      </span>
    </div>
  </div>
</template>

<script setup>
import { defineProps, reactive } from "vue";

// const props = defineProps<{
//   heading?: string;
//   content?: number;
//   id: string;
// }>();

const props = defineProps(["heading", "content", "id"]);

const state = reactive({
  class: "hidden",
  rotation: true,
});

const onShow = () => {
  state.rotation = !state.rotation;

  const accordion = document.getElementById(props.id);
  const panel = accordion.nextElementSibling;

  if (panel.style.maxHeight) {
    panel.style.maxHeight = null;
  } else {
    panel.style.maxHeight = "300px";
  }
};
</script>

<style scoped>
.panel {
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.9s ease-out;
}
</style>
