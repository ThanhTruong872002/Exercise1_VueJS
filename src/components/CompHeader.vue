<template lang="">
  <div class="pt-10 pb-48 bg-black h-auto">
    <div class="container flex justify-between items-center">
      <h1 class="text-white font-bold text-[24px] uppercase">Agency</h1>
      <ul class="text-[16px] flex gap-20 text-white">
        <li class="cursor-pointer">About</li>
        <li class="cursor-pointer">Portfolio</li>
        <li class="cursor-pointer">Contact</li>
      </ul>
    </div>
    <div class="container flex justify-between items-center">
      <div class="z-10">
        <h1
          class="font-bold inknut-antiqua-black text-[110px] font-header mt-24 text-white w-[724px] h-[240px] leading-[10rem]"
        >
          We Create Amazing Sites With Ease
        </h1>
        <div class="mt-36 flex gap-14">
          <img src="/src/images/Flower_decor.svg" alt="" />
          <p class="text-white text-[16px] uppercase w-[370px] leading-[40px]">
            A peep at some distant orb has power to raise and purify
          </p>
        </div>
      </div>
      <div
        class="absolute w-[570px] h-[624px] lg:top-[34%] xl:top-[27%] left-[45%] bg-[#FF564F] flex justify-center items-center"
      >
        <img src="/src/images/Hero_decor1.svg" alt="" class="w-full" />
      </div>
      <div class="translate-y-4">
        <img
          src="/src/images/Combined Shape.svg"
          alt=""
          class="w-[268px] h-[268px]"
        />
      </div>
    </div>
  </div>
  <div class="container">
    <div class="mt-48 flex gap-4 items-center">
      <div
        class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center cursor-pointer"
      >
        <img src="/src/images/Triangle_left.svg" alt="" class="" />
      </div>
      <div
        class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center cursor-pointer"
      >
        <img src="/src/images/Triangle_right.svg" alt="" class="" />
      </div>
      <p class="text-black font-bold text-[24px] ml-6">1 / 2</p>
    </div>

    <div class="w-full h-[2px] bg-black mt-64"></div>
  </div>
</template>

<script>
export default {
  name: "comp-header",
  data() {
    return {
      Text: "Header",
    };
  },
};
</script>
<style lang=""></style>
