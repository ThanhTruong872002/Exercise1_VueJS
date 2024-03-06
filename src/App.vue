<script setup>
import "./assets/main.css";
</script>

<template>
  <header class="pt-10 pb-48 bg-black h-auto">
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
          <img src="../src/images/Flower_decor.svg" alt="" />
          <p class="text-white text-[16px] uppercase w-[370px] leading-[40px]">
            A peep at some distant orb has power to raise and purify
          </p>
        </div>
      </div>
      <div
        class="absolute w-[570px] h-[624px] top-[28%] left-[45%] bg-[#FF564F] flex justify-center items-center"
      >
        <img src="../src/images/Hero_decor1.svg" alt="" class="w-full" />
      </div>
      <div class="translate-y-4">
        <img
          src="../src/images/Combined Shape.svg"
          alt=""
          class="w-[268px] h-[268px]"
        />
      </div>
    </div>
  </header>
  <main class="h-[5000px]">
    <div class="container">
      <div class="mt-48 flex gap-4 items-center">
        <div
          class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center"
        >
          <img src="../src//images/Triangle_left.svg" alt="" />
        </div>
        <div
          class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center"
        >
          <img src="../src//images/Triangle_right.svg" alt="" />
        </div>
        <p class="text-black font-bold text-[24px] ml-6">1 / 2</p>
      </div>

      <div class="w-full h-[2px] bg-black mt-64"></div>
    </div>

    <!-- Take Avantage  -->
    <div class="container">
      <div class="relative mt-40 flex justify-between">
        <div class="">
          <div class="w-[470px] h-[470px] rounded-[50%] bg-[#F8E71C]"></div>
          <div class="absolute -translate-y-[90%] -translate-x-52">
            <img src="../src/images/Take_Avantage.png" alt="" />
          </div>
          <img
            src="../src/images/play.svg"
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
            <button
              class="w-[170px] h-[48px] text-white uppercase bg-[#FF564F]"
            >
              Learn more
            </button>
            <p class="text-[#111111]">Explore services</p>
          </div>
        </div>
      </div>
    </div>

    <!-- Our core Feature  -->
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
          Minuteness of the parts formed a great hindrance to my speed,
          resolved, contrary to my first intention, to make the being.
          Minuteness of the parts formed a great hindrance to my speed,
          resolved, contrary to my first intention, to make the being.
        </p>
      </div>

      <div class="container">
        <div class="mt-32 flex gap-10">
          <div class="w-[570px] bg-[#9013FE] py-20 px-14">
            <img src="../src/images/Feature1.svg" alt="" />
            <h2 class="uppercase py-10 text-white font-bold text-[24px]">
              white lable
            </h2>
            <p class="dm-sans-400 text-[#FFFFFF80]">
              Minuteness of the parts formed a great hindrance to my speed,
              resolved, contrary to my first intention, to make the being.
            </p>
          </div>
          <div class="w-[570px] bg-[#417505] py-20 px-14">
            <img src="../src/images/Feature2.svg" alt="" />
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
          <img src="../src/images/next_item.svg" alt="" />
        </div>
      </div>
    </div>

    <!-- Check Our Project  -->
    <div class="mt-40 py-28">
      <div class="container flex justify-between items-center">
        <h1
          class="inknut-antiqua-black font-[900] text-[7rem] text-black w-[372px] leading-[70px]"
        >
          Our Core Features
        </h1>
        <p class="dm-sans-400 text-[#11111180] w-[570px] leading-[30px]">
          Minuteness of the parts formed a great hindrance to my speed,
          resolved, contrary to my first intention, to make the being.
          Minuteness of the parts formed a great hindrance to my speed,
          resolved, contrary to my first intention, to make the being.
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
                <img src="../src/images/dog1.png" alt="" />
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
                <img src="../src/images/people1.png" alt="" />
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

    <!-- What our clients say  -->
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
                src="../src/images/Ava.svg"
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
              square, was moving across the sand in their direction. When it
              came near enough he perceived that it was not grass; there were no
              blades, but only purple roots. The roots were revolving, for each
              small plant in the whole patch, like the spokes of a rimless
              wheel.
            </p>
          </div>
          <div class="w-[470px] bg-[#9013FE] py-16 px-14">
            <div class="flex gap-4 items-center">
              <img
                src="../src/images/Ava2.svg"
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
              square, was moving across the sand in their direction. When it
              came near enough he perceived that it was not grass; there were no
              blades, but only purple roots. The roots were revolving, for each
              small plant in the whole patch, like the spokes of a rimless
              wheel.
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
          <img src="../src//images/Triangle_left.svg" alt="" />
        </div>
        <div
          class="w-[48px] h-[48px] rounded-[50%] bg-red-500 flex justify-center items-center"
        >
          <img src="../src//images/Triangle_right.svg" alt="" />
        </div>
      </div>

      <div class="w-full h-[2px] bg-black mt-64"></div>
    </div>

    <div class="container">
      <div class="flex items-center justify-between my-32">
        <img src="../src/images/Brand1.svg" alt="" />
        <img src="../src/images/Brand2.svg" alt="" />
        <img src="../src/images/Brand3.svg" alt="" />
        <img src="../src/images/Brand4.svg" alt="" />
        <img src="../src/images/Brand5.svg" alt="" />
      </div>
      <div class="w-full h-[2px] bg-black"></div>

      <div class="flex justify-between items-center mt-40">
        <h1
          class="inknut-antiqua-black font-[900] text-[7rem] text-black w-[372px] leading-[70px]"
        >
          Our latest blog posts
        </h1>
        <p class="dm-sans-400 text-[#11111180] w-[570px] leading-[30px]">
          Minuteness of the parts formed a great hindrance to my speed,
          resolved, contrary to my first intention, to make the being.
          Minuteness of the parts formed a great hindrance to my speed,
          resolved, contrary to my first intention, to make the being.
        </p>
      </div>

      <div class="mt-20 flex gap-6">
        <div class="flex flex-col gap-6">
          <img
            src="../src/images/block1.svg"
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
            src="../src/images/block2.svg"
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
            src="../src/images/block3.svg"
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

    <Footer class="bg-black py-40 mt-40">
      <div class="container">
        <div class="relative">
          <h1
            class="inknut-antiqua-black font-[900] text-[7rem] text-white w-[372px] leading-[70px]"
          >
            Newsletter Sign Up
          </h1>
          <div class="w-full h-[2px] bg-white mt-32"></div>

          <form
            action=""
            class="bg-[#FF564F] w-[470px] px-14 py-20 absolute right-0 -bottom-32"
          >
            <div class="roboto-condensed-500 uppercase text-white">
              Get in touch
            </div>
            <input
              type="text"
              name=""
              id=""
              placeholder="Your email"
              class="p-5 bg-white w-[374px] mt-14"
            />
            <button
              class="uppercase font-bold bg-[#ed6a65] py-5 text-white mt-10 text-center w-[374px]"
            >
              Subscribe
            </button>
          </form>
        </div>

        <div class="mt-48 grid grid-cols-12 text-white">
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
            <img src="../src/images/social.svg" alt="" />
          </div>
        </div>
      </div>
    </Footer>
  </main>
</template>

<style scoped></style>
