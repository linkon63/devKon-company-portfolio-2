<template>
  <div class="bg-[#FFFFFF]">
    <section class="container mx-auto px-6 sm:px-24 flex justify-center">
      <section class="w-full">
        <div class="flex justify-center">
          <div class="">
            <!-- heading section -->
            <div class="grid grid-cols-1 pt-20 2xl:pt-[100px] w-full">
              <div
                class="text-center font-r-semibold text-2xl sm:text-3xl md:text-3xl lg:text-4xl xl:text-[40px] text-[#6E6E73]"
              >
                Know Something More
              </div>
              <div
                class="text-center text-5xl sm:text-6xl md:text-7xl lg:text-[84px] font-r-b pt-6"
              >
                Blog
              </div>
            </div>
          </div>
        </div>
      </section>
    </section>

    <section class="w-6/6 pt-16 2xl:pt-20">
      <!-- :autoplay="{ delay: 1500 }"
      loop -->
      <Swiper
        :space-between="30"
        :modules="[Autoplay]"
        :slidesPerView="3"
        :breakpoints="{
          '100': {
            slidesPerView: 1,
            spaceBetween: 10,
          },
          '200': {
            slidesPerView: 1,
            spaceBetween: 10,
          },
          '400': {
            slidesPerView: 1,
            spaceBetween: 10,
          },
          '640': {
            slidesPerView: 1,
            spaceBetween: 10,
          },
          '768': {
            slidesPerView: 2,
            spaceBetween: 10,
          },
          '1024': {
            slidesPerView: 3,
            spaceBetween: 20,
          },
          '1280': {
            slidesPerView: 4,
            spaceBetween: 30,
          },
          '1536': {
            slidesPerView: 4,
            spaceBetween: 30,
          },
          '1920': {
            slidesPerView: 4,
            spaceBetween: 30,
          },
        }"
      >
        <swiper-slide>
          <div class="box ms-4 bg-[#FAFAFC] rounded-3xl">
            <div class="">
              <div class="">
                <div>
                  <img
                    class="h-[300px] rounded-t-3xl"
                    src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRhOt8yVPy6GGZ4tjCXHpImPPqpNoEwJGeE2Q&s"
                    alt=""
                  />
                </div>
              </div>

              <div class="bg-[#FAFAFC] rounded-b-3xl p-6">
                <div>
                  <h1
                    class="py-4 text-2xl sm:text-3xl font-r-semibold text-left text-[#212121]"
                  >
                    Ea fugiat nobis corrupti excepturi
                  </h1>
                  <p class="text-gray-600 text-left text-xl sm:text-2xl">
                    Lorem Ipsum is simply dummy text of the printing and
                    typesetting.
                  </p>
                  <div class="flex py-4 w-full">
                    <div class="flex items-center w-full sm:w-4/12">
                      <svg
                        fill="#000000"
                        viewBox="0 0 32 32"
                        version="1.1"
                        xmlns="http://www.w3.org/2000/svg"
                        height="28px"
                        width="28px"
                      >
                        <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                        <g
                          id="SVGRepo_tracerCarrier"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        ></g>
                        <g id="SVGRepo_iconCarrier">
                          <title>time1</title>
                          <path
                            d="M16 3.5c-7.181 0-13 5.82-13 13s5.819 13 13 13c7.179 0 13-5.82 13-13s-5.82-13-13-13zM15.895 27.027c-5.799 0-10.5-4.701-10.5-10.5s4.701-10.5 10.5-10.5c5.798 0 10.5 4.701 10.5 10.5s-4.702 10.5-10.5 10.5zM18.93 17.131h-2.98v-5.032c0-0.546-0.443-0.99-0.989-0.99s-0.99 0.443-0.99 0.99v6.021c0 0.547 0.443 0.989 0.99 0.989h3.969c0.547 0 0.99-0.442 0.99-0.989 0-0.546-0.443-0.989-0.99-0.989z"
                          ></path>
                        </g>
                      </svg>
                      <p class="text-gray-600 px-2 w-full text-2xl text-nowrap">
                        2 Min
                      </p>
                    </div>
                  </div>
                </div>
                <div class="flex justify-end px-4 py-[24px]">
                  <ExpandableButton />
                </div>
              </div>
            </div>
          </div>
        </swiper-slide>

        <swiper-slide>
          <div class="box ms-4 bg-[#FAFAFC] rounded-3xl">
            <div class="">
              <div class="">
                <div>
                  <img
                    class="h-[300px] rounded-t-3xl"
                    src="https://cdn.stocksnap.io/img-thumbs/280h/butterflies-nature_IFVYIKNJC1.jpg"
                  />
                </div>
              </div>

              <div class="bg-[#FAFAFC] rounded-b-3xl p-6">
                <div>
                  <h1
                    class="py-4 text-2xl sm:text-3xl font-r-semibold text-left text-[#212121]"
                  >
                    Ea fugiat nobis corrupti excepturi
                  </h1>
                  <p class="text-gray-600 text-left text-xl sm:text-2xl">
                    Lorem Ipsum is simply dummy text of the printing and
                    typesetting.
                  </p>
                  <div class="flex py-4 w-full">
                    <div class="flex items-center w-full sm:w-4/12">
                      <svg
                        fill="#000000"
                        viewBox="0 0 32 32"
                        version="1.1"
                        xmlns="http://www.w3.org/2000/svg"
                        height="28px"
                        width="28px"
                      >
                        <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                        <g
                          id="SVGRepo_tracerCarrier"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        ></g>
                        <g id="SVGRepo_iconCarrier">
                          <title>time1</title>
                          <path
                            d="M16 3.5c-7.181 0-13 5.82-13 13s5.819 13 13 13c7.179 0 13-5.82 13-13s-5.82-13-13-13zM15.895 27.027c-5.799 0-10.5-4.701-10.5-10.5s4.701-10.5 10.5-10.5c5.798 0 10.5 4.701 10.5 10.5s-4.702 10.5-10.5 10.5zM18.93 17.131h-2.98v-5.032c0-0.546-0.443-0.99-0.989-0.99s-0.99 0.443-0.99 0.99v6.021c0 0.547 0.443 0.989 0.99 0.989h3.969c0.547 0 0.99-0.442 0.99-0.989 0-0.546-0.443-0.989-0.99-0.989z"
                          ></path>
                        </g>
                      </svg>
                      <p class="text-gray-600 px-2 w-full text-2xl text-nowrap">
                        2 Min
                      </p>
                    </div>
                  </div>
                </div>
                <div class="flex justify-end px-4 py-[24px]">
                  <ExpandableButton />
                </div>
              </div>
            </div>
          </div>
        </swiper-slide>

        <swiper-slide>
          <div class="box ms-4 bg-[#FAFAFC] rounded-3xl">
            <div class="">
              <div class="rounded-3xl">
                <div>
                  <img
                    class="rounded-t-3xl w-[420px] h-[300px]"
                    src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTvaOwW6DpUGHJ5qzsZRiH9vlJ4rsWgX3vhX_Ve3cFkufO7tLFaGDbv4fBBURRuf8dC_Lg&usqp=CAU"
                    alt=""
                  />
                </div>
              </div>

              <div class="bg-[#FAFAFC] rounded-b-3xl p-6">
                <div>
                  <h1
                    class="py-4 text-2xl sm:text-3xl font-r-semibold text-left text-[#212121]"
                  >
                    Ea fugiat nobis corrupti excepturi
                  </h1>
                  <p class="text-gray-600 text-left text-xl sm:text-2xl">
                    Lorem Ipsum is simply dummy text of the printing and
                    typesetting.
                  </p>
                  <div class="flex py-4 w-full">
                    <div class="flex items-center w-full sm:w-4/12">
                      <svg
                        fill="#000000"
                        viewBox="0 0 32 32"
                        version="1.1"
                        xmlns="http://www.w3.org/2000/svg"
                        height="28px"
                        width="28px"
                      >
                        <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                        <g
                          id="SVGRepo_tracerCarrier"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        ></g>
                        <g id="SVGRepo_iconCarrier">
                          <title>time1</title>
                          <path
                            d="M16 3.5c-7.181 0-13 5.82-13 13s5.819 13 13 13c7.179 0 13-5.82 13-13s-5.82-13-13-13zM15.895 27.027c-5.799 0-10.5-4.701-10.5-10.5s4.701-10.5 10.5-10.5c5.798 0 10.5 4.701 10.5 10.5s-4.702 10.5-10.5 10.5zM18.93 17.131h-2.98v-5.032c0-0.546-0.443-0.99-0.989-0.99s-0.99 0.443-0.99 0.99v6.021c0 0.547 0.443 0.989 0.99 0.989h3.969c0.547 0 0.99-0.442 0.99-0.989 0-0.546-0.443-0.989-0.99-0.989z"
                          ></path>
                        </g>
                      </svg>
                      <p class="text-gray-600 px-2 w-full text-2xl text-nowrap">
                        2 Min
                      </p>
                    </div>
                  </div>
                </div>
                <div class="flex justify-end px-4 py-[24px]">
                  <ExpandableButton />
                </div>
              </div>
            </div>
          </div>
        </swiper-slide>

        <swiper-slide>
          <div class="box ms-4 bg-[#FAFAFC] rounded-b-3xl">
            <div class="">
              <div class="rounded-3xl">
                <div>
                  <img
                    class="rounded-t-3xl h-[300px]"
                    src="https://nt.global.ssl.fastly.net/binaries/content/gallery/website/national/library/our-cause/on-the-shore-borrowdale-and-derwent-water-1518851.jpg?auto=webp&width=767&crop=16:9&dpr=2%202x"
                    alt=""
                  />
                </div>
              </div>

              <div class="p-6">
                <div>
                  <h1
                    class="py-4 text-2xl sm:text-3xl font-r-semibold text-left text-[#212121]"
                  >
                    Ea fugiat nobis corrupti excepturi
                  </h1>
                  <p class="text-gray-600 text-left text-xl sm:text-2xl">
                    Lorem Ipsum is simply dummy text of the printing and
                    typesetting.
                  </p>
                  <div class="flex py-4 w-full">
                    <div class="flex items-center w-full sm:w-4/12">
                      <svg
                        fill="#000000"
                        viewBox="0 0 32 32"
                        version="1.1"
                        xmlns="http://www.w3.org/2000/svg"
                        height="28px"
                        width="28px"
                      >
                        <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                        <g
                          id="SVGRepo_tracerCarrier"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        ></g>
                        <g id="SVGRepo_iconCarrier">
                          <title>time1</title>
                          <path
                            d="M16 3.5c-7.181 0-13 5.82-13 13s5.819 13 13 13c7.179 0 13-5.82 13-13s-5.82-13-13-13zM15.895 27.027c-5.799 0-10.5-4.701-10.5-10.5s4.701-10.5 10.5-10.5c5.798 0 10.5 4.701 10.5 10.5s-4.702 10.5-10.5 10.5zM18.93 17.131h-2.98v-5.032c0-0.546-0.443-0.99-0.989-0.99s-0.99 0.443-0.99 0.99v6.021c0 0.547 0.443 0.989 0.99 0.989h3.969c0.547 0 0.99-0.442 0.99-0.989 0-0.546-0.443-0.989-0.99-0.989z"
                          ></path>
                        </g>
                      </svg>
                      <p class="text-gray-600 px-2 w-full text-2xl text-nowrap">
                        2 Min
                      </p>
                    </div>
                  </div>
                </div>
                <div class="flex justify-end px-4 py-[24px]">
                  <ExpandableButton />
                </div>
              </div>
            </div>
          </div>
        </swiper-slide>

        <swiper-slide>
          <div class="box ms-4 bg-[#FAFAFC] rounded-b-3xl">
            <div class="">
              <div class="rounded-3xl">
                <div>
                  <img
                    class="rounded-t-3xl h-[300px]"
                    src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSKyVfDXaVADLFy6cl9W2BY8AYspIsVQmAfrnRq3vz3wVTcNHZqPBZ0Vt6lof9lWsm5huI&usqp=CAU"
                    alt=""
                  />
                </div>
              </div>

              <div class="p-6">
                <div>
                  <h1
                    class="py-4 text-2xl sm:text-3xl font-r-semibold text-left text-[#212121]"
                  >
                    Ea fugiat nobis corrupti excepturi
                  </h1>
                  <p class="text-gray-600 text-left text-xl sm:text-2xl">
                    Lorem Ipsum is simply dummy text of the printing and
                    typesetting.
                  </p>
                  <div class="flex py-4 w-full">
                    <div class="flex items-center w-full sm:w-4/12">
                      <svg
                        fill="#000000"
                        viewBox="0 0 32 32"
                        version="1.1"
                        xmlns="http://www.w3.org/2000/svg"
                        height="28px"
                        width="28px"
                      >
                        <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                        <g
                          id="SVGRepo_tracerCarrier"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        ></g>
                        <g id="SVGRepo_iconCarrier">
                          <title>time1</title>
                          <path
                            d="M16 3.5c-7.181 0-13 5.82-13 13s5.819 13 13 13c7.179 0 13-5.82 13-13s-5.82-13-13-13zM15.895 27.027c-5.799 0-10.5-4.701-10.5-10.5s4.701-10.5 10.5-10.5c5.798 0 10.5 4.701 10.5 10.5s-4.702 10.5-10.5 10.5zM18.93 17.131h-2.98v-5.032c0-0.546-0.443-0.99-0.989-0.99s-0.99 0.443-0.99 0.99v6.021c0 0.547 0.443 0.989 0.99 0.989h3.969c0.547 0 0.99-0.442 0.99-0.989 0-0.546-0.443-0.989-0.99-0.989z"
                          ></path>
                        </g>
                      </svg>
                      <p class="text-gray-600 px-2 w-full text-2xl text-nowrap">
                        2 Min
                      </p>
                    </div>
                  </div>
                </div>
                <div class="flex justify-end px-4 py-[24px]">
                  <ExpandableButton />
                </div>
              </div>
            </div>
          </div>
        </swiper-slide>

        <swiper-slide>
          <div class="box ms-4 bg-[#FAFAFC] rounded-b-3xl">
            <div class="">
              <div class="rounded-3xl">
                <div>
                  <img
                    class="rounded-t-3xl h-[300px]"
                    src="https://media.istockphoto.com/id/508417878/photo/back-view-of-modern-programmer-sitting-and-writing-code.jpg?s=612x612&w=0&k=20&c=6N-Uxsz3cpAgcqRFN6nq2VVhcuyoSDj-ChXrSzD6eQo="
                    alt=""
                  />
                </div>
              </div>

              <div class="bg-[#FAFAFC] rounded-b-3xl p-6">
                <div>
                  <h1
                    class="py-4 text-2xl sm:text-3xl font-r-semibold text-left text-[#212121]"
                  >
                    Ea fugiat nobis corrupti excepturi
                  </h1>
                  <p class="text-gray-600 text-left text-xl sm:text-2xl">
                    Lorem Ipsum is simply dummy text of the printing and
                    typesetting.
                  </p>
                  <div class="flex py-4 w-full">
                    <div class="flex items-center w-full sm:w-4/12">
                      <svg
                        fill="#000000"
                        viewBox="0 0 32 32"
                        version="1.1"
                        xmlns="http://www.w3.org/2000/svg"
                        height="28px"
                        width="28px"
                      >
                        <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                        <g
                          id="SVGRepo_tracerCarrier"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        ></g>
                        <g id="SVGRepo_iconCarrier">
                          <title>time1</title>
                          <path
                            d="M16 3.5c-7.181 0-13 5.82-13 13s5.819 13 13 13c7.179 0 13-5.82 13-13s-5.82-13-13-13zM15.895 27.027c-5.799 0-10.5-4.701-10.5-10.5s4.701-10.5 10.5-10.5c5.798 0 10.5 4.701 10.5 10.5s-4.702 10.5-10.5 10.5zM18.93 17.131h-2.98v-5.032c0-0.546-0.443-0.99-0.989-0.99s-0.99 0.443-0.99 0.99v6.021c0 0.547 0.443 0.989 0.99 0.989h3.969c0.547 0 0.99-0.442 0.99-0.989 0-0.546-0.443-0.989-0.99-0.989z"
                          ></path>
                        </g>
                      </svg>
                      <p class="text-gray-600 px-2 w-full text-2xl text-nowrap">
                        2 Min
                      </p>
                    </div>
                  </div>
                </div>
                <div class="flex justify-end px-4 py-[24px]">
                  <ExpandableButton />
                </div>
              </div>
            </div>
          </div>
        </swiper-slide>
      </Swiper>

      <div class="flex justify-center items-center py-[70px] h-[186px]">
        <button
          class="flex justify-between items-center px-6 py-[18px] text-black-900 bg-[#E8E8ED] w-[218px] h-[64px] text-[24px] rounded-full"
        >
          <div class="text-[#212121]">See All Blogs</div>
          <p class="">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              strokeWidth="{1.5}"
              stroke="currentColor"
              class="text-2xl"
              height="24px"
              width="24px"
            >
              <path
                strokeLinecap="round"
                strokeLinejoin="round"
                d="M17.25 8.25 21 12m0 0-3.75 3.75M21 12H3"
              />
            </svg>
          </p>
        </button>
      </div>
    </section>
  </div>
</template>
<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay } from "swiper/modules";

import "swiper/css";
import ExpandableButton from "../../buttons/ExpandableButton.vue";
</script>
