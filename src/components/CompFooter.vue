<template lang="">
  <Footer class="bg-black py-40 mt-40">
    <div class="container">
      <div class="relative">
        <h1
          class="inknut-antiqua-black font-[900] text-[50px] lg:text-[7rem] text-white w-[220px] lg:w-[372px] leading-[50px] lg:leading-[70px]"
        >
          Newsletter Sign Up
        </h1>
        <div class="w-full h-[2px] bg-white mt-32"></div>

        <form
          action=""
          class="bg-[#FF564F] w-[320px] lg:w-[470px] px-14 py-20 lg:absolute right-0 -bottom-32"
        >
          <div class="roboto-condensed-500 uppercase text-white">
            Get in touch
          </div>
          <input
            type="text"
            name=""
            id=""
            placeholder="Your email"
            class="p-5 bg-white w-[250px] lg:w-[374px] mt-14"
          />
          <button
            class="uppercase font-bold bg-[#ed6a65] py-5 text-white mt-10 text-center w-[250px] lg:w-[374px]"
          >
            Subscribe
          </button>
        </form>
      </div>

      <div class="mt-48 grid lg:grid-cols-12 text-white gap-20 lg:gap-0">
        <div class="col-span-3">
          <h2>AGENCY</h2>
          <P class="mt-6 w-[140px] text-[#FFFFFF80]"
            >Agency © 2019. All Rights Reserved.</P
          >
        </div>
        <div class="col-span-3 grid gap-4">
          <h2>ADDRESS</h2>
          <p class="mt-6 w-[190px] text-[#FFFFFF80]">
            3899 Fusce Rd. Frederick Nebraska 20620
          </p>
          <p>info@agency.com</p>
          <p>+1 (234) 567-89-00</p>
        </div>
        <div class="col-span-3 grid gap-4">
          <h2>MENU</h2>
          <p class="mt-6 w-[140px] text-[#FFFFFF80]">About</p>
          <p>Portfolio</p>
          <p>Blog</p>
          <p>Testimonials</p>
          <p>Contact</p>
        </div>
        <div class="col-span-3">
          <img src="/src/images/social.svg" alt="" />
        </div>
      </div>
    </div>
  </Footer>
</template>
<script>
export default {
  name: "comp-footer",
  data() {
    return {
      text: "Footer",
    };
  },
};
</script>
<style lang=""></style>
