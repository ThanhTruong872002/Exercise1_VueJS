<template lang="">
  <div class="bg-black mt-40 py-28 overflow-hidden" id="contact">
    <div
      class="container flex flex-col lg:flex-row justify-between items-center"
    >
      <h1
        class="uppercase inknut-antiqua-black font-[900] text-[50px] lg:text-[5.6rem] text-white lg:w-[372px] leading-[50px] lg:leading-[70px]"
      >
        Our Core Features
      </h1>
      <p
        class="text-[16px] dm-sans-400 text-[#FFFFFF80] w-[320px] lg:w-[570px] leading-[30px] mt-20 lg:mt-0"
      >
        Minuteness of the parts formed a great hindrance to my speed, resolved,
        contrary to my first intention, to make the being. Minuteness of the
        parts formed a great hindrance to my speed, resolved, contrary to my
        first intention, to make the being.
      </p>
    </div>

    <div class="container overflow-hidden">
      <div
        :style="{ transform: `translateX(-${slideIndex * 102}%)` }"
        class="mt-48 flex transition-transform duration-500 lg:gap-4 pl-10 gap-5"
      >
        <div v-for="(feature, index) in features" :key="index">
          <div
            class="w-[320px] h-[384px] lg:h-[282px] lg:mr-0 lg:w-[580px] py-20 px-14 -translate-x-12 lg:translate-x-0"
            :class="`${feature.background}`"
          >
            <img :src="feature.image" alt="" />
            <h2 class="uppercase py-10 text-white font-bold text-[24px]">
              {{ feature.title }}
            </h2>
            <p class="dm-sans-400 text-[#FFFFFF80] text-[16px]">
              {{ feature.subTitle }}
            </p>
          </div>
        </div>
      </div>
    </div>
    <!-- Dot buttons -->
    <div class="flex justify-center mt-20 gap-2">
      <button
        v-for="(slide, index) in slides"
        :key="index"
        @click="goToSlide(index)"
        class="focus:bg-violet-700 mx-1 w-4 h-4 bg-white rounded-[50%] mt-6"
      ></button>
    </div>
  </div>
</template>
<script setup>
import { ref, onMounted } from "vue";
import { TEST } from "../constant";

const slideIndex = ref(0);

const features = ref([]);

const slides = ref(Array.from({ length: 3 }, (_, index) => index));

onMounted(async () => {
  try {
    const res = await fetch("data/features.json");
    const result = await res.json();
    features.value = result;
  } catch (error) {
    console.log(error);
  }
});

const goToSlide = (index) => {
  slideIndex.value = index;
};
</script>
