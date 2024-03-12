<template lang="">
  <div class="container">
    <div
      class="mt-[700px] justify-center lg:justify-start lg:mt-40 flex gap-4 items-center"
    >
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
    </div>
  </div>
</template>
<script setup>
import { defineProps } from "vue";

const props = defineProps({
  slideIndex: Number,
});
</script>
<style lang=""></style>
