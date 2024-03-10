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
      slides: [],
      features: [
        {
          image: "./src/images/Feature1.svg",
          title: "WHITE LABEL",
          subTitle:
            "Minuteness of the parts formed a great hindrance to my speed, resolved, contrary to my first intention, to make the being.",
          background: "bg-[#9013FE]",
        },
        {
          image: "./src/images/Feature2.svg",
          title: "CODE EXPORT",
          subTitle:
            "Minuteness of the parts formed a great hindrance to my speed, resolved, contrary to my first intention, to make the being.",
          background: "bg-[#417505]",
        },
        {
          image: "./src/images/Feature1.svg",
          title: "JAVASCRIPT",
          subTitle:
            "Minuteness of the parts formed a great hindrance to my speed, resolved, contrary to my first intention, to make the being.",
          background: "bg-red-500",
        },
        {
          image: "./src/images/Feature2.svg",
          title: "PYTHON",
          subTitle:
            "Minuteness of the parts formed a great hindrance to my speed, resolved, contrary to my first intention, to make the being.",
          background: "bg-blue-200",
        },
        {
          image: "./src/images/Feature1.svg",
          title: "WHITE LABEL",
          subTitle:
            "Minuteness of the parts formed a great hindrance to my speed, resolved, contrary to my first intention, to make the being.",
          background: "bg-[#9013FE]",
        },
        {
          image: "./src/images/Feature2.svg",
          title: "CODE EXPORT",
          subTitle:
            "Minuteness of the parts formed a great hindrance to my speed, resolved, contrary to my first intention, to make the being.",
          background: "bg-[#417505]",
        },
      ],
    };
  },
  mounted() {
    this.slides = Array.from(
      { length: this.features.length },
      (_, index) => index
    );
  },
  methods: {
    goToSlide(index) {
      this.slideIndex = index;
    },
  },
};
</script>
<style lang=""></style>
