<template lang="">
  <div class="pt-10 lg:pb-48 bg-black h-auto">
    <div class="container flex justify-between items-center">
      <h1 class="text-white font-bold lg:text-[24px] uppercase md:text-[16px]">
        Agency
      </h1>
      <div>
        <div class="lg:hidden cursor-pointer" @click="toggleMenu">
          <img src="/src/images/menu.svg" alt="" class="w-[30px] h-[28px]" />
        </div>
        <div
          v-if="isOpen === true"
          class="lg:hidden w-[300px] h-auto right-10 translate-y-4 bg-white absolute rounded-lg z-30"
        >
          <div
            class="w-full text-center font-bold p-5 hover:bg-orange-500 cursor-pointer"
          >
            About
          </div>
          <div
            class="w-full text-center font-bold p-5 hover:bg-orange-500 cursor-pointer"
          >
            Portfolio
          </div>
          <div
            class="w-full text-center font-bold p-5 hover:bg-orange-500 cursor-pointer"
          >
            Contact
          </div>
        </div>
      </div>
      <div class="hidden text-[16px] lg:flex gap-20 text-white">
        <a href="#about" class="cursor-pointer">About</a>
        <a href="#portfolio" class="cursor-pointer">Portfolio</a>
        <a href="#contact" class="cursor-pointer">Contact</a>
      </div>
    </div>

    <div class="w-[100vw] lg:h-[72vh] overflow-hidden">
      <div
        :style="{ transform: `translateX(-${slideIndex * 50}%)` }"
        class="flex transition-transform duration-500 w-[200vw]"
      >
        <!-- Slide 1 -->
        <div class="w-full">
          <div
            class="container flex-col flex lg:flex-row justify-between items-center"
          >
            <div class="z-10">
              <h1
                class="font-bold inknut-antiqua-black text-[50px] lg:text-[110px] font-header mt-24 text-white w-[312px] lg:w-[724px] h-[192px] lg:h-[240px] leading-[6rem] lg:leading-[10rem]"
              >
                We Create Amazing Sites With Ease
              </h1>
              <div class="lg:mt-36 mt-10 flex gap-14">
                <img src="/src/images/Flower_decor.svg" alt="" />
                <p
                  class="text-white text-[16px] uppercase w-[229px] lg:w-[370px] leading-[40px]"
                >
                  A peep at some distant orb has power to raise and purify
                </p>
              </div>
            </div>
            <div
              class="relative w-[329px] h-[360px] mt-40 lg:mt-0 lg:absolute lg:w-[570px] lg:h-[624px] lg:top-[34%] xl:top-[40%] lg:left-[23%] bg-[#FF564F] flex justify-center items-center"
            >
              <img src="/src/images/Hero_decor1.svg" alt="" class="w-full" />
            </div>
            <div
              class="lg:translate-y-4 lg:translate-x-0 -translate-y-[215%] translate-x-[60%]"
            >
              <img
                src="/src/images/Combined Shape.svg"
                alt=""
                class="w-[268px] h-[208px]"
              />
            </div>
          </div>
        </div>
        <!-- Slide 2 -->
        <div class="w-full">
          <div
            class="container flex-col flex lg:flex-row justify-between items-center overflow-hidden"
          >
            <div class="z-20">
              <h1
                class="font-bold inknut-antiqua-black text-[50px] lg:text-[110px] font-header mt-24 text-white w-[312px] lg:w-[724px] h-[192px] lg:h-[240px] leading-[6rem] lg:leading-[10rem]"
              >
                We Create Amazing Sites With Ease
              </h1>
              <div class="lg:mt-36 mt-10 flex gap-14">
                <img src="/src/images/Flower_decor.svg" alt="" />
                <p
                  class="text-white text-[16px] uppercase w-[229px] lg:w-[370px] leading-[40px]"
                >
                  A peep at some distant orb has power to raise and purify
                </p>
              </div>
            </div>
            <div
              class="relative w-[329px] h-[360px] mt-40 lg:mt-0 lg:absolute lg:w-[570px] lg:h-[624px] lg:top-[34%] xl:top-[40%] lg:right-[12%] bg-orange-300 flex justify-center items-center z-10"
            >
              <img src="/src/images/Hero_decor1.svg" alt="" class="w-full" />
            </div>
            <div
              class="lg:translate-y-4 lg:translate-x-0 -translate-y-[215%] translate-x-[60%] z-0"
            >
              <img
                src="/src/images/Combined Shape.svg"
                alt=""
                class="w-[268px] h-[208px]"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="container">
    <div class="mt-2 lg:mt-10 flex gap-4 items-center">
      <div
        @click="prevSlide"
        class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center cursor-pointer"
      >
        <img src="/src/images/Triangle_left.svg" alt="" class="" />
      </div>
      <div
        @click="nextSlide"
        class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center cursor-pointer"
      >
        <img src="/src/images/Triangle_right.svg" alt="" class="" />
      </div>
      <p class="text-black font-bold text-[24px] ml-6">
        {{ slideIndex + 1 }} / 2
      </p>
    </div>

    <div class="w-full h-[2px] bg-black mt-40 lg:mt-64"></div>
  </div>
</template>

<script>
export default {
  name: "comp-header",
  data() {
    return {
      text: "Header",
      isOpen: false,
      slideIndex: 0,
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
  },
};
</script>
<style lang=""></style>
