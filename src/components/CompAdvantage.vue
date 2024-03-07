<template lang="">
  <div class="container" id="advantage">
    <div
      class="relative mt-40 flex flex-col gap-20 lg:gap-0 lg:flex-row lg:justify-between"
    >
      <div >
        <div
          class=" w-[320px] h-[320px] lg:w-[470px] lg:h-[470px] rounded-[50%] bg-[#F8E71C]"
        ></div>
        <div
          class="absolute -translate-y-[120%] lg:-translate-y-[90%] lg:-translate-x-52"
        >
          <img
            src="/src/images/Take_Avantage.png"
            alt=""
            class="lg:w-[676px] lg:h-[557px] w-[340px] h-[260px]"
          />
        </div>
        <img
          src="/src/images/play.svg"
          alt=""
          class="absolute top-28 left-28 lg:top-52 lg:left-52 cursor-pointer"
        />
      </div>
      <div class="">
        <h1
          class="text-[#111111] inknut-antiqua-black text-[40px] lg:text-[56px] font-[800] uppercase w-[320px]  lg:w-[449px]"
        >
          Lets Take Advantage
        </h1>
        <p
          class="roboto-condensed-500 text-[16px] text-[#111111] uppercase font-bold my-10"
        >
          sable cloud beneath was dished
        </p>
        <p
          class="dm-sans-400 font-[16px] text-[#11111180] w-[329px] lg:w-[470px] leading-[4rem]"
        >
          Best for active freelancers and designers who need more projects and
          premium features code and unlock more.
        </p>
        <div class="flex gap-10 mt-10 items-center">
          <button class="w-[170px] h-[48px] text-white uppercase bg-[#FF564F]">
            Learn more
          </button>
          <div class="text-[#111111] w-[140px]">Explore services</div>
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
