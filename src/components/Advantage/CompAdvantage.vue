<template lang="">
  <div class="container" id="advantage">
    <div
      class="relative mt-40 flex flex-col gap-20 lg:gap-0 lg:flex-row lg:justify-between"
    >
      <div v-if="!showVideo">
        <div
          class="w-[320px] h-[320px] lg:w-[470px] lg:h-[470px] rounded-[50%] bg-[#F8E71C] z-50"
        ></div>
        <div class="absolute top-5 lg:-top-16 lg:-translate-x-52">
          <img src="/src/assets/images/Bitmap2.png" alt="" class=" " />
        </div>
        <img
          @click="playVideo"
          src="/src/assets/images/play.svg"
          alt=""
          class="absolute top-28 left-28 lg:top-52 lg:left-52 cursor-pointer"
        />
      </div>
      <div v-if="showVideo" class="relative">
        <iframe
          src="https://www.youtube.com/embed/dQw4w9WgXcQ"
          title="YouTube video player"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen
          class="w-[100%] lg:w-[500px] lg:h-[500px]"
        >
        </iframe>
        <svg
          @click="closeVideo"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-12 h-12 font-bold cursor-pointer absolute -top-10 -right-12"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M6 18 18 6M6 6l12 12"
          />
        </svg>
      </div>

      <div>
        <h1
          class="text-[#111111] inknut-antiqua-black text-[40px] lg:text-[56px] font-[800] uppercase w-[320px] lg:w-[449px]"
        >
          Lets Take Advantage
        </h1>
        <p
          class="roboto-condensed-500 text-[16px] text-[#111111] uppercase font-semibold my-10"
        >
          sable cloud beneath was dished
        </p>
        <p
          class="dm-sans-400 text-[16px] text-[#11111180] w-[329px] lg:w-[470px] leading-[4rem]"
        >
          Best for active freelancers and designers who need more projects and
          premium features code and unlock more.
        </p>
        <div class="flex gap-10 mt-10 items-center">
          <button
            class="w-[170px] h-[48px] text-white uppercase bg-[#FF564F] font-bold text-[17px] roboto-condensed hover:opacity-80 hover:p-6"
          >
            Learn more
          </button>
          <div
            class="text-[#111111] w-[140px] text-[16px] dm-sans cursor-pointer hover:opacity-80 hover:text-red-800"
          >
            Explore services
          </div>
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
      showVideo: false,
    };
  },
  methods: {
    playVideo() {
      this.showVideo = true;
    },
    closeVideo() {
      this.showVideo = false;
    },
  },
};
</script>
<style lang=""></style>
