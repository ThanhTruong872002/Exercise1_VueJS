<template lang="">
  <div class="bg-black mt-40 py-28">
    <div class="container flex justify-between items-center">
      <h1
        class="inknut-antiqua-black font-[900] text-[7rem] text-white w-[372px] leading-[70px]"
      >
        Our Core Features
      </h1>
      <p
        class="text-white dm-sans-400 text-[#FFFFFF80] w-[570px] leading-[30px]"
      >
        Minuteness of the parts formed a great hindrance to my speed, resolved,
        contrary to my first intention, to make the being. Minuteness of the
        parts formed a great hindrance to my speed, resolved, contrary to my
        first intention, to make the being.
      </p>
    </div>

    <div class="container">
      <div class="mt-32 flex gap-10">
        <div class="w-[570px] bg-[#9013FE] py-20 px-14">
          <img src="/src/images/Feature1.svg" alt="" />
          <h2 class="uppercase py-10 text-white font-bold text-[24px]">
            white lable
          </h2>
          <p class="dm-sans-400 text-[#FFFFFF80]">
            Minuteness of the parts formed a great hindrance to my speed,
            resolved, contrary to my first intention, to make the being.
          </p>
        </div>
        <div class="w-[570px] bg-[#417505] py-20 px-14">
          <img src="/src/images/Feature2.svg" alt="" />
          <h2 class="uppercase py-10 text-white font-bold text-[24px]">
            code export
          </h2>
          <p class="dm-sans-400 text-[#FFFFFF80]">
            Minuteness of the parts formed a great hindrance to my speed,
            resolved, contrary to my first intention, to make the being.
          </p>
        </div>
      </div>
      <div class="flex justify-center mt-20">
        <img src="/src/images/next_item.svg" alt="" />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "comp-feature",
  data() {
    return {
      text: "Our Core Feature",
    };
  },
};
</script>
<style lang=""></style>
