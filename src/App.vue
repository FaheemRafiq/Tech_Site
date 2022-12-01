<template>
  <div>
    <landing-vue/>
    <Features/>
  </div>
</template>

<script>
import LandingVue from './pages/Landing.vue';
import Features from './pages/Features.vue'
import Landing from './pages/Landing.vue';
export default {
  components:{Features , LandingVue},
  setup(){
    Landing
  }
}
</script>

<style>

</style>