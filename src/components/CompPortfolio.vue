<template lang="">
  <div class="mt-40 py-28">
    <div class="container flex justify-between items-center">
      <h1
        class="inknut-antiqua-black font-[900] text-[7rem] text-black w-[372px] leading-[70px]"
      >
        Our Core Features
      </h1>
      <p class="dm-sans-400 text-[#11111180] w-[570px] leading-[30px]">
        Minuteness of the parts formed a great hindrance to my speed, resolved,
        contrary to my first intention, to make the being. Minuteness of the
        parts formed a great hindrance to my speed, resolved, contrary to my
        first intention, to make the being.
      </p>
    </div>
    <div class="container">
      <div class="w-full m-auto h-[2px] bg-black mt-40"></div>
    </div>

    <div class="container">
      <div class="grid grid-cols-12 mt-32">
        <div class="col-span-4">
          <h2 class="mb-10 roboto-condensed-500 text-[#111111] uppercase">
            Portfolio
          </h2>
          <ul class="flex flex-col gap-6">
            <li
              class="bg-[#111111] w-[170px] h-[48px] text-white cursor-pointer rounded-s flex items-center justify-items-start pl-6"
            >
              All
            </li>
            <li
              class="w-[170px] h-[48px] text-black bg-white cursor-pointer flex items-center justify-items-start pl-6"
            >
              Design
            </li>
            <li
              class="w-[170px] h-[48px] text-black bg-white cursor-pointer flex items-center justify-items-start pl-6"
            >
              Development
            </li>
            <li
              class="w-[170px] h-[48px] text-black bg-white cursor-pointer flex items-center justify-items-start pl-6"
            >
              Branding
            </li>
            <li
              class="w-[170px] h-[48px] text-black bg-white cursor-pointer flex items-center justify-items-start pl-6"
            >
              Products
            </li>
          </ul>
        </div>

        <div class="col-span-8">
          <div class="w-full relative h-[416px] bg-[#F8E71C]">
            <div class="flex flex-col gap-8 pl-10">
              <div class="mt-96">
                <p class="uppercase roboto-condensed-500 text-[#111111]">
                  design
                </p>
                <h2
                  class="uppercase inknut-antiqua-black text-[40px] w-[281px] font-[900] text-[#111111]"
                >
                  Creative Template
                </h2>
              </div>
            </div>
            <div class="absolute right-0 -top-20">
              <img src="/src/images/dog1.png" alt="" />
            </div>
          </div>

          <div class="w-full relative h-[416px] bg-[#FF564F] mt-28">
            <div class="flex flex-col gap-8 pl-10">
              <div class="mt-96">
                <p class="uppercase roboto-condensed-500 text-white">
                  Branding
                </p>
                <h2
                  class="uppercase inknut-antiqua-black text-[40px] w-[281px] font-[900] text-white"
                >
                  Amazing Startup
                </h2>
              </div>
            </div>
            <div class="absolute -right-28 -top-7">
              <img src="/src/images/people1.png" alt="" />
            </div>
          </div>
          <div class="text-center">
            <button
              class="mt-20 w-[170px] h-[48px] font-medium text-[16px] text-white uppercase bg-[#FF564F]"
            >
              Load more
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "comp-portfolio",
  data() {
    return {
      text: "portfolio",
    };
  },
};
</script>
<style lang=""></style>
