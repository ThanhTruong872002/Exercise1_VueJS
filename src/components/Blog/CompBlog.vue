<template lang="">
  <div class="container">
    <div class="w-full h-[2px] bg-black mt-20 lg:mt-64 lg:mb-40"></div>
    <div
      class="flex flex-col lg:flex-row items-center justify-between my-32 gap-32 lg:gap-0 mt-40 lg:mt-0"
    >
      <div
        v-for="(item, index) in brands"
        class="cursor-pointer hover:opacity-70"
      >
        <a :href="item.link" target="_blank"
          ><img :src="`${item.image}`" alt="Brand Logo"
        /></a>
      </div>
    </div>
    <div class="w-full h-[2px] bg-black"></div>

    <div class="flex flex-col lg:flex-row justify-between items-center mt-40">
      <h1
        class="inknut-antiqua-black text-[40px] lg:text-[5.6rem] uppercase text-black w-[330px] lg:w-[460px] leading-[50px] lg:leading-[70px]"
      >
        Our latest blog posts
      </h1>
      <p
        class="dm-sans-400 text-[#11111180] w-[300px] lg:w-[570px] leading-[30px] mt-10 lg:mt-0 text-[1.6rem]"
      >
        Minuteness of the parts formed a great hindrance to my speed, resolved,
        contrary to my first intention, to make the being. Minuteness of the
        parts formed a great hindrance to my speed, resolved, contrary to my
        first intention, to make the being.
      </p>
    </div>

    <div class="mt-20 flex flex-col lg:flex-row gap-20 lg:gap-10 text-[1.6rem]">
      <div v-for="(itemBlog, index) in blogs" class="flex flex-col gap-6">
        <img
          :src="itemBlog.image"
          alt=""
          class="w-[370px] h-[288px] object-cover hover:p-2 cursor-pointer"
        />
        <h2 class="roboto-condensed-500 uppercase">{{ itemBlog.title }}</h2>
        <h1 class="text-[#111111] uppercase font-bold w-[330px]">
          {{ itemBlog.description }}
        </h1>
        <p class="font-[400] text-[#11111180]">{{ itemBlog.date }}</p>
      </div>
    </div>
  </div>
</template>
<script setup>
import { ref, onMounted } from "vue";

const blogs = ref([]);

const brands = ref([]);

onMounted(async () => {
  try {
    const res = await fetch("data/blogs.json");
    const result = await res.json();
    blogs.value = result;
  } catch (error) {
    console.log(error);
  }
});

onMounted(async () => {
  try {
    const res = await fetch("data/brands.json");
    const result = await res.json();
    brands.value = result;
  } catch (error) {
    console.log(error);
  }
});
</script>
<style lang=""></style>
