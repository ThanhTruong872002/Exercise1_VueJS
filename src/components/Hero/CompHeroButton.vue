<template lang="">
  <div class="container">
    <div class="mt-96 lg:mt-40 flex gap-4 items-center">
      <div
        @click="$emit('prevSlide')"
        class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center cursor-pointer"
      >
        <img src="/src/assets/images/Triangle_left.svg" alt="" class="" />
      </div>
      <div
        @click="$emit('nextSlide')"
        class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center cursor-pointer"
      >
        <img src="/src/assets/images/Triangle_right.svg" alt="" class="" />
      </div>
      <p class="text-black font-bold text-[24px] ml-6">{{slideIndex + 1}}/ {{ bannersLength }}</p>
    </div>
    <div class="w-full h-[2px] bg-black mt-40 lg:mt-96"></div>
  </div>
</template>
<script>
export default {
  name: "comp-hero-button",
  props: {
    slideIndex: Number,
    bannersLength: Number,
  },
};
</script>
<style lang=""></style>
