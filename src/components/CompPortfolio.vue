<template lang="">
  <div class="lg:mt-40 mt-20 py-28 container" id="portfolio">
    <div class="">
      <div
        class="flex flex-col lg:flex-row justify-between items-center gap-10 lg:gap-0"
      >
        <h1
          class="inknut-antiqua-black font-[900] text-[50px] w-full lg:text-[7rem] text-black lg:w-[372px] leading-[50px] lg:leading-[70px]"
        >
          Check Our Projects
        </h1>
        <p class="dm-sans-400 text-[#11111180] lg:w-[570px] leading-[30px]">
          Minuteness of the parts formed a great hindrance to my speed,
          resolved, contrary to my first intention, to make the being.
          Minuteness of the parts formed a great hindrance to my speed,
          resolved, contrary to my first intention, to make the being.
        </p>
      </div>
    </div>
    <div class="">
      <div class="w-full m-auto h-[2px] bg-black mt-40"></div>
    </div>

    <div class="">
      <div class="grid lg:grid-cols-12 mt-32">
        <div class="col-span-4">
          <h2 class="mb-10 roboto-condensed-500 text-[#111111] uppercase">
            Portfolio
          </h2>
          <ul class="hidden lg:flex flex-col gap-6">
            <li
              class="w-[170px] h-[48px] cursor-pointer rounded-s flex items-center justify-items-start pl-6"
              v-for="(category, index) in allCategories"
              :key="index"
              :class="{ active: selectedItemIndex === index }"
              @click="selectItem(index)"
            >
              {{ category }}
            </li>
          </ul>

          <div
            class="lg:hidden w-[320px] p-5 border-[1px] border-[#ccc] border-solid flex justify-between items-center"
          >
            <p>All</p>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="w-6 h-6 cursor-pointer"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="m19.5 8.25-7.5 7.5-7.5-7.5"
              />
            </svg>
          </div>
        </div>

        <div class="col-span-8 mt-40 lg:mt-0">
          <div
            v-if="selectedItemIndex === 1 || selectedItemIndex === 0"
            class="w-full relative h-[416px] bg-[#F8E71C]"
          >
            <div class="flex flex-col gap-8 pl-10">
              <div class="mt-96 z-20">
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
            <div class="absolute top-8 lg:right-0 lg:-top-20">
              <img src="/src/images/dog1.png" alt="" class=" " />
            </div>
          </div>

          <div
            v-if="selectedItemIndex === 2 || selectedItemIndex === 0"
            class="w-full lg:relative h-[416px] bg-[#FF564F] mt-28 overflow-hidden"
          >
            <div class="flex flex-col gap-8 pl-10">
              <div class="mt-96 z-20">
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
            <div
              class="lg:absolute lg:right-0 lg:-top-7 relative bottom-96 z-10"
            >
              <img
                src="/src/images/people1.png"
                alt=""
                class="w-[320px] h-[330px] lg:w-[614px] lg:h-[435px] object-cover"
              />
            </div>
          </div>

          <div
            v-if="isLoadMore === true"
            class="w-full lg:relative h-[416px] bg-[#2f6850] mt-28 overflow-hidden"
          >
            <div class="flex flex-col gap-8 pl-10">
              <div class="mt-96 z-20">
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
            <div
              class="lg:absolute lg:right-0 lg:-top-7 relative bottom-96 z-10"
            >
              <img
                src="/src/images/people1.png"
                alt=""
                class="w-[320px] h-[330px] lg:w-[614px] lg:h-[435px] object-cover"
              />
            </div>
          </div>
          <div class="text-center">
            <button
              @click="handleLoadMore"
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
      isLoadMore: false,
      selectedItemIndex: 0,
      allCategories: ["All", "Design", "Branding", "Development", "Products"],
    };
  },
  methods: {
    handleLoadMore() {
      this.isLoadMore = true;
    },
    selectItem(index) {
      this.selectedItemIndex = index;
    },
  },
};
</script>
<style lang="scss">
li.active {
  background-color: #111111;
  color: #ffffff;
}
</style>
