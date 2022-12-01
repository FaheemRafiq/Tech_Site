<script>
import LandingVue from './pages/Landing.vue';
import Features from './pages/Features.vue'
import FooterVue from './pages/Footer.vue';
export default {
  components:{Features , LandingVue , FooterVue},
}
</script>

<template>
  <div>
    <landing-vue/>
    <Features/>
    <footer-vue/>
  </div>
</template>
