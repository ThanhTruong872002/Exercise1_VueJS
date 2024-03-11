<template lang="">
  <div class="container">
    <div class="w-full h-[2px] bg-black mt-64 mb-40"></div>
    <div
      class="flex flex-col lg:flex-row items-center justify-between my-32 gap-32 lg:gap-0 mt-80 lg:mt-0"
    >
      <div
        v-for="(item, index) in brand"
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
<script>
import Brand1 from "/src/assets/images/Brand1.svg"
export default {
  name: "comp-blog",
  data() {
    return {
      brand: [
        {
          image: Brand1,
          link: "https://www.atlassian.com/git/tutorials/syncing/git-pull",
        },
        {
          image: "/src/images/Brand2.svg",
          link: "https://www.bing.com/search?pglt=41&q=slack&cvid=c9980da298bb43be807f911bab27e39b&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIGCAEQABhAMgYIAhAAGEAyBggDEAAYQDIGCAQQABhAMgYIBRAAGEAyBggGEAAYQDIGCAcQABhAMgYICBAAGEDSAQg0MzcxajBqMagCALACAA&FORM=ANNTA1&adppc=EDGEESS&PC=EDGEESS",
        },
        {
          image: "/src/images/Brand3.svg",
          link: "https://www.dropbox.com/",
        },
        {
          image: "/src/images/Brand4.svg",
          link: "https://www.shopify.com/free-trial/3s?gclid=17bfd3e6b02314f2b192b60a8cc9c074&gclsrc=3p.ds&&utm_medium=cpc&utm_source=yabing&jk=shopify&utm_source=yabing&utm_medium=cpc&utm_campaign=429206062&bingadgroupid=1230353764689029&bingadid=76897258418057&bingkeywordid=76897314828284&bingnetwork=o&BOID=brand&msclkid=17bfd3e6b02314f2b192b60a8cc9c074&utm_term=shopify&utm_content=Brand%20-%20Shopify",
        },
        {
          image: "/src/images/Brand5.svg",
          link: "https://www.google.com/",
        },
      ],
      blogs: [
        {
          title: "design",
          description: "Truly it was a great journey and in it I met with many",
          date: "14 November, 2019",
          image: "/src/images/block1.svg",
        },
        {
          title: "tech",
          description: "What looked like a small patch of purple grass",
          date: "14 November, 2019",
          image: "/src/images/block2.svg",
        },
        {
          title: "life",
          description: "The roots were revolving small plant",
          date: "14 November, 2019",
          image: "/src/images/block3.svg",
        },
      ],
    };
  },
};
</script>
<style lang=""></style>
