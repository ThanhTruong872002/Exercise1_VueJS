<template lang="">
  <div class="bg-black lg:pb-40 z-10">
    <div class="container overflow-x-clip">
      <div
        :style="{ transform: `translateX(-${slideIndex * 105}%)` }"
        class="transition-transform duration-500 flex gap-10 lg:gap-0"
      >
        <div v-for="(banner, index) in banners" :key="index" class="px-2">
          <div class="relative flex flex-col lg:flex-row lg:w-[1220px] mr-5">
            <div class="z-10">
              <div class="flex flex-col">
                <h1
                  class="max-md:w-[312px] lg:w-[724px] text-[40px] lg:text-[7.2rem] inknut-antiqua-black text-white lg:leading-[80px] uppercase"
                >
                  {{ banner.title }}
                </h1>
                <div class="lg:mt-16 mt-10 flex gap-14">
                  <img src="/src/assets/images/Flower_decor.svg" alt="" />
                  <p
                    class="text-white text-[16px] uppercase w-[229px] lg:w-[370px] leading-[40px] roboto-condensed tracking-[2px]"
                  >
                    {{ banner.subtitle }}
                  </p>
                </div>
              </div>
            </div>
            <div
              class="mt-10 lg:mt-0 relative lg:absolute lg:right-0 lg:top-10 z-0 w-[268px] h-[268px]"
            >
              <img
                src="/src/assets/images/Combined Shape.svg"
                alt=""
                class="translate-x-64 lg:translate-x-0"
              />
              <div
                class="absolute top-32 lg:top-[35%] lg:right-[50%] w-[320px] h-[360px] lg:w-[570px] lg:h-[624px] z-10"
                :class="`${banner.background}`"
              >
                <img
                  src="/src/assets/images/Hero_decor1.svg"
                  alt=""
                  class="absolute -top-[20%] lg:top-[10%] h-[513px]"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <comp-hero-button
    @nextSlide="nextSlide"
    @prevSlide="prevSlide"
    :slideIndex="slideIndex"
    :bannersLength="banners.length"
  />
</template>
<script>
import CompHeroButton from "./CompHeroButton.vue";
import { ref } from "vue";
export default {
  name: "comp-hero",
  components: {
    CompHeroButton,
  },
  data() {
    return {
      slideIndex: ref(0),
      banners: [
        {
          title: "We Create Amazing Sites With Ease",
          subtitle: " A peep at some distant orb has power to raise and purify",
          background: "bg-[#FF564F]",
        },
        {
          title: "We Create Amazing Sites With Ease",
          subtitle: " A peep at some distant orb has power to raise and purify",
          background: "bg-[#ccc]",
        },
      ],
    };
  },
  methods: {
    nextSlide() {
      this.slideIndex = (this.slideIndex + 1) % this.banners.length;
    },
    prevSlide() {
      if (this.slideIndex !== 0) {
        this.slideIndex = (this.slideIndex - 1) % this.banners.length;
      }
    },
  },
};
</script>
<style lang=""></style>
