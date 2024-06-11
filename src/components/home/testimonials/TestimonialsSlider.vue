<template>
  <div class="flex justify-around h-[500px] main relative">
    <div class="hidden lg:block">
      <div class="w-full h-full">
        <div class="absolute top-1/4">
          <button
            class="group w-[52px] h-[52px] rounded-full bg-[#9AC7FF] hover:bg-[#EEEEEE] flex justify-center items-center"
            @click="prev()"
          >
            <span>
              <img
                class="group-hover:hidden -rotate-[0deg]"
                src="../../../assets/images/home/arrow_left_blue.png"
                width="14px"
                height="14px"
              />
              <img
                class="hidden group-hover:block rotate-[0deg]"
                src="../../../assets/images/home/Testimonials/left-arrow-black-icon.png"
                width="14px"
                height="14px"
              />
            </span>
          </button>
        </div>
      </div>
    </div>
    <Carousel
      ref="myCarousel"
      :itemsToShow="5"
      :wrapAround="true"
      :transition="500"
      class="w-10/12"
      :breakpoints="{
        100: {
          itemsToShow: 1,
          snapAlign: 'start',
        },
        700: {
          itemsToShow: 2.5,
          snapAlign: 'center',
        },
        1024: {
          itemsToShow: 3,
        },
        1440: {
          itemsToShow: 5,
        },
      }"
    >
      <Slide v-for="slide in state.slider" :key="slide">
        <!-- style="border: 5px solid green" -->
        <div class="carousel__item relative">
          <div class="flex justify-center mySlide p-0 relative">
            <div class="mySlideContent p-0 relative mt-3">
              <div class="flex justify-center items-center p-0">
                <img
                  :src="slide.image"
                  alt="testimonial images"
                  class="w-[200px] h-[200px] rounded-full text-center c-img"
                />
              </div>
            </div>
          </div>
          <p
            class="text-[32px] text-nowrap font-r-semibold pt-[52px] title px-4"
          >
            {{ slide.title }}
          </p>
          <p class="description">
            {{ slide.desciption }}
          </p>
        </div>
      </Slide>
      <template #addons>
        <Pagination class="pagination" />
      </template>
    </Carousel>
    <div class="hidden lg:block">
      <div class="w-full h-full">
        <div class="absolute top-1/4 right-16">
          <button
            class="group w-[52px] h-[52px] rounded-full bg-[#0567E1] hover:bg-[#EEEEEE] flex justify-center items-center"
            @click="next()"
          >
            <span>
              <img
                class="group-hover:hidden -rotate-[0deg]"
                src="../../../assets/images/home/Testimonials/white-left-arrow-icon.png"
                width="14px"
                height="14px"
              />
              <img
                class="hidden group-hover:block rotate-[180deg]"
                src="../../../assets/images/home/Testimonials/left-arrow-black-icon.png"
                width="14px"
                height="14px"
              />
            </span>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { defineComponent, onMounted, reactive } from "vue";
import { Carousel, Pagination, Slide } from "vue3-carousel";
import { ref } from "vue";

import "vue3-carousel/dist/carousel.css";

const myCarousel = ref(null);

const state = reactive({
  slider: [
    {
      id: 1,
      title: "Industry Expertise &",
      desciption:
        "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry.",
      image:
        "https://images.unsplash.com/photo-1464863979621-258859e62245?q=80&w=1886&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    },
    {
      id: 2,
      title: "Industry Expertise &",
      desciption:
        "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry.",
      image:
        "https://images.unsplash.com/photo-1438761681033-6461ffad8d80?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    },
    {
      id: 3,
      title: "Industry Expertise &",
      desciption:
        "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry.",
      image:
        "https://media.istockphoto.com/id/637359514/photo/teenager-girl-cute-beautiful-freckles-face-on-white.jpg?s=2048x2048&w=is&k=20&c=tcd_YClwdUdQYHRmTeM_GXIfs443wslAk2E-95Z1rbU=",
    },

    {
      id: 4,
      title: "Industry Expertise &",
      desciption:
        "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry.",
      image:
        "https://media.istockphoto.com/id/637359364/photo/teenager-girl-cute-beautiful-freckles-face-on-white.jpg?s=2048x2048&w=is&k=20&c=EFl0wgfsCAKRAX3VOMWlXgGQmhclunUAysJvjlz6Ibk=",
    },

    {
      id: 5,
      title: "Industry Expertise &",
      desciption:
        "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry.",
      image:
        "https://images.unsplash.com/photo-1529626455594-4ff0802cfb7e?q=80&w=1887&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    },
  ],
});

const prev = () => {
  myCarousel.value.prev();
  paginationStyle();
};

const next = () => {
  myCarousel.value.next();
  // console.log('next value');
  // // paginationStyle()
  // let button = document.querySelectorAll(".carousel__pagination-button");
  // console.log('button value', button);

  // for (let i = 0; i < button.length; i++) {
  //   const element = button[i];
  //   element.style.border = "3px solid #DEDEDE";
  //   element.style.borderRadius = "50%";
  //   element.style.width = "12px";
  //   element.style.height = "12px";
  //   element.style.backgroundColor = "#DEDEDE";
  //   element.style.margin = "8px";

  //   element.classList.remove("carousel__pagination-button");
  //   console.log('el', element);
  // }

  // let active = document.querySelector(".carousel__pagination-button--active");
  //   active.style.backgroundColor = "blue";
  //   active.style.borderColor = "blue";
};

onMounted(() => {
  // paginationStyle();
  // let active = document.querySelector(".carousel__pagination-button--active");
  //   active.style.backgroundColor = "blue";
  //   active.style.borderColor = "blue";
});

const paginationStyle = () => {
  let button = document.querySelectorAll(".carousel__pagination-button");
  for (let i = 0; i < button.length; i++) {
    const element = button[i];
    element.style.border = "3px solid #DEDEDE";
    element.style.borderRadius = "50%";
    element.style.width = "12px";
    element.style.height = "12px";
    element.style.backgroundColor = "#DEDEDE";
    element.style.margin = "8px";

    element.classList.remove("carousel__pagination-button");
  }
};
</script>

<style scoped lang="scss">
.pagination {
  padding-bottom: 52px;
}
.carousel__item {
  min-height: 00px;
  width: 600px;
  border-radius: 8px;
}
.carousel__slide {
  padding: 1px;
}

.carousel__viewport {
  perspective: 1500px;
}

.carousel__track {
  height: 700px !important;
  transform-style: preserve-3d;
  position: relative;
}

.carousel__slide--sliding {
  transition: 0.5s;
}

.carousel__slide {
  opacity: 0.9;
  transform: rotateY(-20deg) scale(0.6);
}

.carousel__slide--active ~ .carousel__slide {
  transform: rotateY(20deg) scale(0.6);
}

.carousel__slide--prev {
  opacity: 1;
  transform: rotateY(-10deg) scale(0.7);
  margin: 0% 0% !important;
}

.carousel__slide > .carousel__item > p {
  display: none;
}

.carousel__slide--prev > .carousel__item > p {
  display: none;
}

.carousel__slide--next > .carousel__item > p {
  display: none;
}

.carousel__slide--active > .carousel__item > p {
  display: block;
}

.carousel__slide--next {
  opacity: 1;
  transform: rotateY(10deg) scale(0.7) !important;
}

.description {
  position: absolute;
  left: -45%;
  margin: 20px 0;
  width: 800px;
  font-size: 24px;
}

.carousel__slide--active {
  opacity: 1;
  transform: rotateY(0) scale(1);
  margin: 0% 40px;
  position: relative;
}

.title {
  font-size: 32px;
}

.carousel__pagination {
  margin-top: 10px;
}

.carousel__slide--active {
  opacity: 1;
  margin: 0% 0%;
}

@media only screen and (min-width: 150px) and (max-width: 250px) {
  .carousel__item {
    text-align: center;
  }
}

@media only screen and (min-width: 150px) and (max-width: 320px) {
  .carousel__item {
    min-height: 300px;
    width: 300px;
    border-radius: 8px;
    margin-left: 60%;
    /* background: rgb(8, 163, 41); */
  }

  .c-img {
    height: 100px;
    width: 100px;
  }
  .title {
    font-size: 16px;
  }
  .description {
    font-size: 16px;
    position: relative;
    left: 0;
    width: auto !important;
  }
  .carousel__slide--active {
    opacity: 1;
    /* transform: rotateY(0) scale(1); */
    margin: 0% 0%;
  }
  .main {
    height: 400px;
  }

  .carousel__slide {
    margin: 0% -3%;
  }

  .carousel__pagination {
    margin-top: 10px;
  }
}

@media only screen and (min-width: 320px) and (max-width: 481px) {
  .carousel__item {
    min-height: 300px;
    width: 300px;
    border-radius: 8px;
    margin-left: 45%;
    /* background: red; */
  }

  .c-img {
    height: 100px;
    width: 100px;
  }
  .title {
    font-size: 16px;
  }
  .description {
    font-size: 16px;
    position: relative;
    left: 0;
    width: auto !important;
  }
  .carousel__slide--active {
    opacity: 1;
    /* transform: rotateY(0) scale(1); */
    margin: 0% 0%;
  }
  .main {
    height: 400px;
  }

  .carousel__slide {
    margin: 0% -2.2%;
  }
}

/* @media screen and (min-width: 200px) {
  
} */

@media screen and (min-width: 482px) {
  .carousel__item {
    min-height: 400px;
    width: 400px;
    border-radius: 8px;
  }

  .description {
    font-size: 24px;
    position: relative;
    left: 0;
    width: auto;
  }

  .carousel__slide {
    margin: 0% 0%;
  }
}

@media screen and (min-width: 768px) {
  .description {
    font-size: 32px;
    position: relative;
    left: 0;
  }
  .carousel__item {
    min-height: 400px;
    width: 400px;
    border-radius: 8px;
  }
  .title {
    font-size: 32px;
  }

  .description {
    position: absolute;
    left: -45%;
    margin: 20px 0;
    width: 600px;
    font-size: 24px;
  }
  .carousel__slide {
    margin: 0% 0%;
  }
  .carousel__pagination {
    position: relative;
    margin-top: 100px;
    margin: 52px 0;
    padding-bottom: 52px;
  }
}

@media only screen and (min-width: 1025px) and (max-width: 1200px) {
  .description {
    position: absolute;
    left: -45%;
    margin: 20px 0;
    width: 600px;
    font-size: 24px;
  }
  .carousel__pagination {
    position: relative;
    margin-top: 100px;
    margin: 52px 0;
    padding-bottom: 52px;
  }
}

@media only screen and (min-width: 1250px) and (max-width: 1440px) {
  .description {
    position: absolute;
    left: -45%;
    margin: 20px 18%;
    width: 600px;
    font-size: 24px;
  }
  .carousel__pagination {
    position: relative;
    margin-top: 100px;
    margin: 52px 0;
    padding-bottom: 52px;
  }
}

@media only screen and (min-width: 1025px) and (min-width: 1441px) {
  .description {
    position: absolute;
    left: -45%;
    margin: 20px 0;
    width: 600px;
    font-size: 24px;
  }
  .carousel__pagination {
    position: relative;
    margin-top: 100px;
    margin: 52px 0;
    padding-bottom: 52px;
  }
}
</style>
