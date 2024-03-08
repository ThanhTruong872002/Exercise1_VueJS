<template lang="">
  <div class="bg-black mt-40 py-28 overflow-hidden" id="contact">
    <div
      class="container flex flex-col lg:flex-row justify-between items-center"
    >
      <h1
        class="inknut-antiqua-black font-[900] text-[50px] lg:text-[7rem] text-white lg:w-[372px] leading-[50px] lg:leading-[70px]"
      >
        Our Core Features
      </h1>
      <p
        class="text-white dm-sans-400 text-[#FFFFFF80] w-[320px] lg:w-[570px] leading-[30px] mt-20 lg:mt-0"
      >
        Minuteness of the parts formed a great hindrance to my speed, resolved,
        contrary to my first intention, to make the being. Minuteness of the
        parts formed a great hindrance to my speed, resolved, contrary to my
        first intention, to make the being.
      </p>
    </div>

    <div class="lg:w-[100vw] overflow-hidden">
      <div
        :style="{ transform: `translateX(-${slideIndex * 50}%)` }"
        class="flex transition-transform duration-500 w-[200vw] mt-32"
      >
        <div class="w-full ">
          <div class=" container px-10">
            <div class="flex gap-4 ">
              <div
                class="w-[320px]  lg:h-[282px] lg:mr-0 h-[384px] lg:w-[570px] bg-[#9013FE] py-20 px-14 -translate-x-12 lg:translate-x-0"
              >
                <img src="/src/images/Feature1.svg" alt="" />
                <h2 class="uppercase py-10 text-white font-bold text-[24px]">
                  white label
                </h2>
                <p class="dm-sans-400 text-[#FFFFFF80]">
                  Minuteness of the parts formed a great hindrance to my speed,
                  resolved, contrary to my first intention, to make the being.
                </p>
              </div>
              <div
                class="w-[320px] translate-x-12 h-[384px] lg:h-[282px] lg:w-[570px] ml-16 lg:ml-0 bg-[#417505] py-20 px-14 lg:translate-x-0"
              >
                <img src="/src/images/Feature2.svg" alt="" />
                <h2 class="uppercase py-10 text-white font-bold text-[24px]">
                  code export
                </h2>
                <p class="dm-sans-400 text-[#FFFFFF80]">
                  Minuteness of the parts formed a great hindrance to my speed,
                  resolved, contrary to my first intention, to make the being.
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="w-full">
          <div class="container">
            <div class="flex gap-4">
              <div class="w-[570px] bg-yellow-400 py-20 px-14">
                <img src="/src/images/Feature1.svg" alt="" />
                <h2 class="uppercase py-10 text-white font-bold text-[24px]">
                  white label
                </h2>
                <p class="dm-sans-400 text-[#FFFFFF80]">
                  Minuteness of the parts formed a great hindrance to my speed,
                  resolved, contrary to my first intention, to make the being.
                </p>
              </div>
              <div class="w-[570px] bg-rose-500 py-20 px-14">
                <img src="/src/images/Feature2.svg" alt="" />
                <h2 class="uppercase py-10 text-white font-bold text-[24px]">
                  code export
                </h2>
                <p class="dm-sans-400 text-[#FFFFFF80]">
                  Minuteness of the parts formed a great hindrance to my speed,
                  resolved, contrary to my first intention, to make the being.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Dot buttons -->
    <div class="flex justify-center mt-4">
      <button
        v-for="(slide, index) in slides"
        :key="index"
        @click="goToSlide(index)"
        :class="{
          'text-white': index === slideIndex,
          'text-gray-400': index !== slideIndex,
        }"
        class="focus:bg-violet-700 mx-1 w-4 h-4 bg-white rounded-[50%] mt-6"
      ></button>
    </div>
  </div>
</template>
<script>
export default {
  name: "comp-feature",
  data() {
    return {
      text: "Our Core Feature",
      slideIndex: 0,
      slides: [0, 4],
    };
  },
  methods: {
    toggleMenu() {
      this.isOpen = !this.isOpen;
    },
    nextSlide() {
      this.slideIndex = (this.slideIndex + 1) % 2;
    },
    prevSlide() {
      this.slideIndex = (this.slideIndex - 1 + 2) % 2;
    },
    goToSlide(index) {
      this.slideIndex = index;
    },
  },
};
</script>
<style lang=""></style>
