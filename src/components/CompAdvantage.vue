<template lang="">

   <div class="container">
    <div class="relative mt-40 flex justify-between">
      <div class="">
        <div class="w-[470px] h-[470px] rounded-[50%] bg-[#F8E71C]"></div>
        <div class="absolute -translate-y-[90%] -translate-x-52">
          <img src="/src/images/Take_Avantage.png" alt="" />
        </div>
        <img
          src="/src/images/play.svg"
          alt=""
          class="absolute top-52 left-52"
        />
      </div>
      <div>
        <h1
          class="text-[#111111] inknut-antiqua-black text-[56px] font-[800] uppercase w-[449px]"
        >
          Lets Take Advantage
        </h1>
        <p
          class="roboto-condensed-500 text-[16px] text-[#111111] uppercase font-bold my-10"
        >
          sable cloud beneath was dished
        </p>
        <p
          class="dm-sans-400 font-[16px] text-[#11111180] w-[470px] leading-[4rem]"
        >
          Best for active freelancers and designers who need more projects and
          premium features code and unlock more.
        </p>
        <div class="flex gap-10 mt-10 items-center">
          <button class="w-[170px] h-[48px] text-white uppercase bg-[#FF564F]">
            Learn more
          </button>
          <p class="text-[#111111]">Explore services</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "comp-advantage",
  data() {
    return {
      text: "Lets take advantage",
    };
  },
};
</script>
<style lang=""></style>
