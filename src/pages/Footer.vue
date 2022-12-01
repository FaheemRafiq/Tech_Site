<script setup>
import ButtonVue from "../components/Button.vue";
</script>

<template>
  <div class="bg-black text-white pb-10" id="contact">
    <section>
      <h3 class="uppercase text-center">35,000 already joined</h3>
      <h1 class="font-bold text-xl md:text-2xl text-center mt-6">
        Stay up-to-date with what we're doing
      </h1>
      <div class="text-center mt-4">
        <input
          class="p-2 w-7/12 md:w-1/3 lg:w-1/4 rounded-md text-black font-light"
          type="email"
          placeholder="Enter your email address"
        />
        <ButtonVue class="ml-4" name="Join us" />
      </div>
    </section>
    <div class="flex flex-col sm:flex-row md:mx-10 lg:mx-60 items-center sm:justify-between mt-10">
      <div class="flex items-center w-9/12 sm:w-1/2 justify-around">
        <img src="../assets/images/podcast.png" width="50" />
        <nav class="w-9/12 xl:w-1/2 flex justify-between">
          <a href="#features">Features</a>
          <a href="#pricing">Pricing</a>
          <a href="#contact">contact</a>
        </nav>
      </div>
      <div class="flex justify-around w-32 mt-10 sm:mt-0">
        <img src="../assets/twitter.svg" width="35" alt="Twitter" />
        <img src="../assets/facebook-logo-2019.svg" width="35" alt="Facrbook" />
      </div>
    </div>
  </div>
</template>
