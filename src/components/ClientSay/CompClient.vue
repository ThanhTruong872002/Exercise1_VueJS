<template lang="">
  <div class="lg:relative lg:overflow-hidden pb-20" id="about">
    <div class="bg-black h-[440px] py-60">
      <div
        class="container flex flex-col lg:flex-row justify-between items-center"
      >
        <div>
          <h1
            class="inknut-antiqua-black text-[40px] lg:text-[5.6rem] text-white w-[325px] lg:w-[455px] leading-[40px] uppercase lg:leading-[60px]"
          >
            What Our Clients Say
          </h1>
          <p
            class="roboto-condensed text-[1.6rem] text-white uppercase font-normal tracking-[3px] mt-20"
          >
            Testimonials
          </p>
        </div>

        <div class="container overflow-hidden">
          <div
            class="gap-4 relative lg:absolute lg:-right-96 lg:top-[20%] w-[940px] text-[16px]"
          >
            <div class="w-full flex lg:gap-6">
              <div v-for="(item, index) in clientSay" :key="index">
                <div
                  class="w-[329px] lg:h-auto lg:w-[470px] py-16 px-8 lg:px-14 mt-20 lg:mt-0"
                  :class="`${item.background}`"
                >
                  <div class="flex gap-4 items-center">
                    <img
                      :src="item.image"
                      alt=""
                      class="rounded-[50%] object-cover"
                    />
                    <div>
                      <h2 class="uppercase font-bold text-[24px text-white">
                        {{ item.name }}
                      </h2>
                      <p class="text-white mt-2">{{ item.company }}</p>
                    </div>
                  </div>
                  <p
                    class="text-[#FFFFFF80] dm-sans-400 mt-60 leading-[35px] w-[235px] lg:w-auto"
                  >
                    {{ item.desc }}
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <CompClientButton
      @nextSlide="nextSlide"
      @prevSlide="prevSlide"
      :slideIndex="slideIndex"
    />
  </div>
  <CompBlog />
</template>
<script setup>
import CompBlog from "../Blog/CompBlog.vue";
import CompClientButton from "./CompClientButton.vue";
import { ref, onMounted } from "vue";

const clientSay = ref([]);

onMounted(async () => {
  try {
    const res = await fetch("data/clients.json");
    const result = await res.json();
    clientSay.value = result;
  } catch (error) {
    console.log(error);
  }
});

const nextSlide = () => {
  const firstItem = clientSay.value[0];
  clientSay.value.shift();
  clientSay.value.push(firstItem);
};

const prevSlide = () => {
  const lastIndex = clientSay.value.length - 1;
  const lastItem = clientSay.value[lastIndex];
  clientSay.value.pop();
  clientSay.value.unshift(lastItem);
};
</script>
<style lang="css"></style>
