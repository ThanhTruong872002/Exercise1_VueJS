<template lang="">
  <div class="bg-black py-60 relative">
    <div class="container flex justify-between items-center">
      <h1
        class="inknut-antiqua-black font-[900] text-[7rem] text-white w-[372px] leading-[70px]"
      >
        What Our Clients Say
      </h1>
      <div class="flex gap-4 absolute -right-96 top-[30%]">
        <div class="w-[470px] bg-[#417505] py-16 px-14">
          <div class="flex gap-4 items-center">
            <img
              src="/src/images/Ava.svg"
              alt=""
              class="rounded-[50%] object-cover"
            />
            <div>
              <h2 class="uppercase font-bold text-[24px text-white">
                Helena Brauer
              </h2>
              <p class="text-white mt-2">Apple Inc.</p>
            </div>
          </div>
          <p class="text-[#FFFFFF80] dm-sans-400 mt-60 leading-[35px]">
            What looked like a small patch of purple grass, above five feet
            square, was moving across the sand in their direction. When it came
            near enough he perceived that it was not grass; there were no
            blades, but only purple roots. The roots were revolving, for each
            small plant in the whole patch, like the spokes of a rimless wheel.
          </p>
        </div>
        <div class="w-[470px] bg-[#9013FE] py-16 px-14">
          <div class="flex gap-4 items-center">
            <img
              src="/src/images/Ava2.svg"
              alt=""
              class="rounded-[50%] object-cover"
            />
            <div>
              <h2 class="uppercase font-bold text-[24px text-white">
                Kay Totleben
              </h2>
              <p class="text-white mt-2">Microsoft</p>
            </div>
          </div>
          <p class="text-[#FFFFFF80] dm-sans-400 mt-60 leading-[35px]">
            What looked like a small patch of purple grass, above five feet
            square, was moving across the sand in their direction. When it came
            near enough he perceived that it was not grass; there were no
            blades, but only purple roots. The roots were revolving, for each
            small plant in the whole patch, like the spokes of a rimless wheel.
          </p>
        </div>
      </div>
    </div>
  </div>

  <div class="container">
    <div class="mt-48 flex gap-4 items-center">
      <div
        class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center"
      >
        <img src="/src//images/Triangle_left.svg" alt="" />
      </div>
      <div
        class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center"
      >
        <img src="/src//images/Triangle_right.svg" alt="" />
      </div>
    </div>

    <div class="w-full h-[2px] bg-black mt-64"></div>
  </div>

  <div class="container">
    <div class="flex items-center justify-between my-32">
      <img src="/src/images/Brand1.svg" alt="" />
      <img src="/src/images/Brand2.svg" alt="" />
      <img src="/src/images/Brand3.svg" alt="" />
      <img src="/src/images/Brand4.svg" alt="" />
      <img src="/src/images/Brand5.svg" alt="" />
    </div>
    <div class="w-full h-[2px] bg-black"></div>

    <div class="flex justify-between items-center mt-40">
      <h1
        class="inknut-antiqua-black font-[900] text-[7rem] text-black w-[372px] leading-[70px]"
      >
        Our latest blog posts
      </h1>
      <p class="dm-sans-400 text-[#11111180] w-[570px] leading-[30px]">
        Minuteness of the parts formed a great hindrance to my speed, resolved,
        contrary to my first intention, to make the being. Minuteness of the
        parts formed a great hindrance to my speed, resolved, contrary to my
        first intention, to make the being.
      </p>
    </div>

    <div class="mt-20 flex gap-6">
      <div class="flex flex-col gap-6">
        <img
          src="/src/images/block1.svg"
          alt=""
          class="w-[370px] h-[288px] object-cover"
        />
        <h2 class="roboto-condensed-500">Design</h2>
        <h1 class="text-[#111111] uppercase font-bold">
          Truly it was a great journey and in it I met with many
        </h1>
        <p class="font-[400] text-[#11111180]">14 November, 2019</p>
      </div>
      <div class="flex flex-col gap-6">
        <img
          src="/src/images/block2.svg"
          alt=""
          class="w-[370px] h-[288px] object-cover"
        />
        <h2 class="roboto-condensed-500">Tech</h2>
        <h1 class="text-[#111111] uppercase font-bold">
          What looked like a small patch of purple grass
        </h1>
        <p class="font-[400] text-[#11111180]">14 November, 2019</p>
      </div>
      <div class="flex flex-col gap-6">
        <img
          src="/src/images/block3.svg"
          alt=""
          class="w-[370px] h-[288px] object-cover"
        />
        <h2 class="roboto-condensed-500">Life</h2>
        <h1 class="text-[#111111] uppercase font-bold">
          The roots were revolving small plant
        </h1>
        <p class="font-[400] text-[#11111180]">14 November, 2019</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "comp-client",
  data() {
    return {
      text: "Client",
    };
  },
};
</script>
<style lang=""></style>
