<template lang="">
  <div class="container">
    <div class="mt-96 lg:mt-40 flex gap-4 items-center">
      <div
        @click="$emit('prevSlide')"
        class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center cursor-pointer"
      >
        <img src="/src/images/Triangle_left.svg" alt="" class="" />
      </div>
      <div
        @click="$emit('nextSlide')"
        class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center cursor-pointer"
      >
        <img src="/src/images/Triangle_right.svg" alt="" class="" />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "comp-client-button",
  props: {
    slideIndex: Number,
  },
};
</script>
<style lang=""></style>
