<template lang="">
  <Footer class="bg-black py-40 mt-40">
    <div class="container">
      <div class="relative">
        <h1
          class="inknut-antiqua-black text-[35px] lg:text-[5.2rem] uppercase text-white w-[213px] lg:w-[460px] leading-[50px] lg:leading-[70px]"
        >
          Newsletter Sign Up
        </h1>
        <div class="w-full h-[2px] bg-white mt-32"></div>

        <form
          action=""
          class="bg-[#FF564F] w-[320px] lg:w-[470px] px-14 py-20 lg:absolute right-0 -bottom-32 text-[1.6rem]"
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
            class="uppercase font-bold bg-[#ed6a65] py-5 text-white mt-10 text-center w-[250px] lg:w-[374px] hover:opacity-75"
          >
            Subscribe
          </button>
        </form>
      </div>

      <div
        class="mt-48 grid lg:grid-cols-12 text-white gap-20 lg:gap-0 text-[1.6rem]"
      >
        <div class="col-span-3">
          <h2>AGENCY</h2>
          <P class="mt-6 w-[140px] text-[#FFFFFF80]"
            >Agency © 2019. All Rights Reserved.</P
          >
        </div>
        <div class="col-span-3 grid gap-4">
          <h2>ADDRESS</h2>
          <p class="mt-6 w-[190px] text-[#FFFFFF80] cursor-pointer">
            3899 Fusce Rd. Frederick Nebraska 20620
          </p>
          <p class="cursor-pointer">info@agency.com</p>
          <a class="cursor-pointer">+1 (234) 567-89-00</a>
        </div>
        <div class="col-span-3 grid gap-4">
          <p>MENU</p>
          <p class="mt-6 w-[140px] text-[#FFFFFF80] cursor-pointer">About</p>
          <a href="#portfolio" class="cursor-pointer">Portfolio</a>
          <a class="cursor-pointer">Blog</a>
          <a class="cursor-pointer">Testimonials</a>
          <a href="#contact" class="cursor-pointer">Contact</a>
        </div>
        <div class="col-span-3">
          <a href="https://www.facebook.com/profile.php?id=100012255758419" target="_blank"><img src="/src/images/social.svg" alt="" /></a>
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
