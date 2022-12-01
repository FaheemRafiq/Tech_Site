<script >
import ButtonVue from "./Button.vue";
import NavVue from "./Nav.vue";
import { ref } from "vue";
export default {
  components: { ButtonVue, NavVue },
  setup() {
    const navShow = ref(false);
    return { navShow };
  },
  methods: {},
};
</script>

<template>
  <header
    class="
      bg-black
      text-white
      flex
      justify-center
      md:items-end
      h-40
      w-full
      text-sm
    "
  >
    <div class="pb-6 w-9/12 md:w-full lg:w-9/12 xl:w-10/12 md:px-4 flex items-center">
      <!-- img div -->
      <div class="">
        <img
          src="../assets/images/podcast.png"
          class="h-16 w-16"
          alt="Logo png"
        />
      </div>
      <!-- Bar For Small Devices -->
      <div class="ml-auto md:hidden">
        <button type="button" @click="navShow = true" class="cursor-pointer">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-10 h-10"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
            />
          </svg>
        </button>
      </div>
      <!-- Navigation For Large Screen Devices -->
      <div class="ml-auto w-1/2 xl:w-1/3 md:flex md:items-center hidden ">
        <nav class="flex w-full lg:w-9/12 justify-around uppercase mr-5 mt-1">
          <a href="#features">Features</a>
          <a href="#pricing">Pricing</a>
          <a href="#contact">Contact</a>
        </nav>
        <ButtonVue name="login" />
      </div>
    </div>
  </header>
  <nav-vue :display="navShow" @close="navShow = false" />
</template>

<style>
</style>