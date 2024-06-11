<template>
  <footer class="">
    <!-- card section start -->
    <div class="container px-6 md:px-24 mx-auto flex justify-center h-[250px]">
      <div class="relative w-[960px]">
        <div class="absolute top-[25%]">
          <div
            class="grid grid-cols-1 sm:flex sm:justify-end footer-card bg-white rounded-3xl"
          >
            <div class="w-1/12 sm:w-4/12"></div>
            <div
              class="pt-10 lg:pt-[86px] pr-[52px] w-11/12 md:w-9/12 lg:w-[58%]"
            >
              <p class="text-2xl md:text-[52px] font-r-b text-right">
                Have an Idea?
              </p>
              <p
                class="text-lg md:text-[32px] pt-5 text-right"
                style="line-height: 44px"
              >
                Do you have any idea to share, Don’t waste you time and talk
                with us.
              </p>
              <div class="pb-[57px] text-right">
                <button
                  class="text-xl py-3 px-9 mt-[52px] rounded-full animate-btn"
                >
                  Let's Talk
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- fotter section man start -->
    <div class="bg-[#F3F4F4]">
      <div
        class="container px-6 sm:px-24 mx-auto flex justify-center py-4 md:pb-16 pt-[250px] sm:pt[280px] lg:pt-[290px]"
      >
        <div class="">
          <div
            class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-6 lg:gap-8"
          >
            <div>
              <div>
                <img
                  src="../../assets/images/home/Softzino Logo.png"
                  class="w-[130px]"
                  alt=""
                />
              </div>
              <div class="text-gray-700 text-[16px] py-8 text-left">
                Lorem Ipsum is simply dummy text of the printing and typesetting
                industry. Lorem Ipsum has been the industry’s standard dummy
                text ever since the 1500s, when an unknown printer took a galley
                of type and scrambled it to make a type specimen book.
              </div>
            </div>

            <div class="py-0 sm:py-2 md:py-4 lg:py-14">
              <div class="font-r-semibold text-gray-700">
                Mobile Development
              </div>
              <p class="text-gray-700 text-[16px] pt-3">
                React Native Development
              </p>
              <p class="text-gray-700 text-[16px] pt-3">
                Flutter App Development
              </p>
              <p class="text-gray-700 text-[16px] pt-3">
                Native Android Development
              </p>
              <p class="text-gray-700 text-[16px] pt-3">
                Native IOS Development
              </p>

              <div class="font-r-semibold text-gray-700 pt-4">
                Software Development
              </div>
              <div class="font-r-semibold text-gray-700 pt-4">MVP Development</div>
              <div class="font-r-semibold text-gray-700 pt-4">Q/A Testing</div>
            </div>
            <div class="py-0 sm:py-2 md:py-4 lg:py-14">
              <div class="font-r-semibold text-gray-700">Web Development</div>
              <p class="text-gray-700 text-[16px] pt-3">React Development</p>
              <p class="text-gray-700 text-[16px] pt-3">Node.js Development</p>
              <p class="text-gray-700 text-[16px] pt-3">Angular Development</p>
              <p class="text-gray-700 text-[16px] pt-3">PHP Development</p>
              <p class="text-gray-700 text-[16px] pt-3">Durpal Development</p>
              <p class="text-gray-700 text-[16px] pt-3">Python Development</p>
              <p class="text-gray-700 text-[16px] pt-3">Laravel Development</p>
              <p class="text-gray-700 text-[16px] pt-3">Java Development</p>

              <div class="font-r-semibold text-gray-700 pt-4">
                Full Stack Development
              </div>
            </div>
            <div class="py-0 sm:py-2 md:py-4 lg:py-14">
              <div class="font-r-semibold text-gray-700">Digital Marketing</div>
              <p class="text-gray-700 text-[16px] pt-3">SEO Service</p>
              <p class="text-gray-700 text-[16px] pt-3">SMS Service</p>
              <p class="text-gray-700 text-[16px] pt-3">PPC Service</p>
              <p class="text-gray-700 text-[16px] pt-3">
                App Marketing Service
              </p>
              <div class="font-r-semibold text-gray-700 pt-4">
                App Development
              </div>
              <div class="font-r-semibold text-gray-700 pt-4">CMS Development</div>
            </div>

            <div class="py-0 sm:py-2 md:py-4 lg:py-14">
              <div class="font-r-semibold text-gray-700">Our Company</div>
              <p class="text-gray-700 text-[16px] pt-3">About us</p>
              <p class="text-gray-700 text-[16px] pt-3">Why choose us</p>
              <p class="text-gray-700 text-[16px] pt-3">Carrier</p>
              <p class="text-gray-700 text-[16px] pt-3">Event and Activities</p>
              <p class="text-gray-700 text-[16px] pt-3">The Tradeshow</p>
              <p class="text-gray-700 text-[16px] pt-3">Blog</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <nav class="bg-white py-3 mb-0 text-center">
      <p class="text-[14px]">
        © 2024 Softzino Technologies, All Rights Reserved.
      </p>
    </nav>
  </footer>
</template>

<script setup></script>

<style scoped>
.footer-card {
  background-image: url("../../assets/images/home/footer-section/fotterImg.png");
  background-size: 442.65px 280px;
  background-repeat: no-repeat;
  background-position: 6% 95%;
}

.animate-btn {
  border: 2px solid #d109b6;
  color: #fff;
  background: linear-gradient(90deg, #9513d1, #d109b6, #9513d1, #d109b6);
  background-size: 400% 400%;
  animation: gradientBG 2s ease infinite;
  cursor: pointer;
}

@media screen and (max-width: 1023px) {
  .footer-card {
    background-size: 280px 180px;
  }
}

@media screen and (max-width: 510px) {
  .footer-card {
    background: none;
    background: white;
  }
}


@keyframes gradientBG {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
</style>
