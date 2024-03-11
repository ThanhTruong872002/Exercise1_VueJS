<template lang="">
  <div class="pt-10 pb-40 bg-black h-auto overflow-hidden">
    <div class="container flex justify-between items-center">
      <h1 class="text-white font-bold lg:text-[24px] uppercase text-[16px]">
        Agency
      </h1>
      <div>
        <div class="lg:hidden cursor-pointer" @click="toggleMenu">
          <img src="/src/assets/images/menu.svg" alt="" class="w-[30px] h-[28px]" />
        </div>
        <div
          v-if="isOpen === true"
          class="lg:hidden w-[300px] h-auto right-10 translate-y-4 bg-white absolute rounded-lg z-30 text-[1.6rem]"
        >
          <div
            class="w-full text-center font-bold p-5 hover:bg-orange-500 cursor-pointer hover:opacity-75 hover:text-red-700"
          >
            <a href="#about"> About </a>
          </div>
          <div
            class="w-full text-center font-bold p-5 hover:bg-orange-500 cursor-pointer hover:opacity-75 hover:text-red-700"
          >
            <a href="#portfolio"> Portfolio </a>
          </div>
          <div
            class="w-full text-center font-bold p-5 hover:bg-orange-500 cursor-pointer hover:opacity-75 hover:text-red-700"
          >
            <a href="#contact"> Contact </a>
          </div>
        </div>
      </div>
      <div class="hidden text-[16px] lg:flex gap-20 text-white">
        <a
          href="#about"
          class="cursor-pointer hover:opacity-75 hover:text-red-700"
          >About</a
        >
        <a
          href="#portfolio"
          class="cursor-pointer hover:opacity-75 hover:text-red-700"
          >Portfolio</a
        >
        <a
          href="#contact"
          class="cursor-pointer hover:opacity-75 hover:text-red-700"
          >Contact</a
        >
      </div>
    </div>
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
