<script setup>
import HeaderVue from "../components/Header.vue";
import ButtonVue from "../components/Button.vue";
</script>


<template>
  <section>
    <header-vue />
    <div class="bg-black text-white flex justify-center items-center">
      <div
        class="
          flex flex-col
          items-center
          lg:flex-row
          md:py-20
          lg:py-30 lg:px-20
        "
      >
        <div
          class="
            text-center
            lg:text-left
            py-10
            order-2
            lg:order-1
            w-9/12
            md:w-1/2
          "
        >
          <h1 class="text-3xl font-bold text-gray-200 pb-4">
            The ultimate USB microphone
          </h1>
          <p class="pb-4 text-gray-500">
            Create incomparable recordings with your computer. Yeti microphones
            produce pristine, studio-quality recordings with legendary ease.
          </p>
          <ButtonVue name="discover" blue />
        </div>
        <div class="w-1/2 flex justify-center lg:order-2">
          <img
            src="../assets/images/chris-yang.png"
            width="350"
            height="250"
            class="z-10"
            alt="Mic"
          />
        </div>
        <!-- Bg blue Color Mic -->
        <div
          class="
            absolute
            lg:w-[55%]
            xl:w-2/4
            h-60
            bg-[#5267DF]
            right-0
            top-[470px]
            z-1
            rounded-tl-full rounded-bl-full
          "
        ></div>
      </div>
    </div>
    <svg class="absolute" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path
        fill="#000000"
        fill-opacity="1"
        d="M0,160L48,160C96,160,192,160,288,144C384,128,480,96,576,80C672,64,768,64,864,58.7C960,53,1056,43,1152,80C1248,117,1344,203,1392,245.3L1440,288L1440,0L1392,0C1344,0,1248,0,1152,0C1056,0,960,0,864,0C768,0,672,0,576,0C480,0,384,0,288,0C192,0,96,0,48,0L0,0Z"
      ></path>
    </svg>
  </section>
</template>
