<template>
  <div id="home">
    <Hero />
    <Brands />
    <Features />
    <Banner />
    <Footer />
  </div>
</template>

<script>
import Hero from "@/components/landing/Hero.vue";
import Brands from "@/components/landing/Brands.vue";
import Features from "@/components/landing/Features.vue";
import Banner from "@/components/landing/Banner.vue";
import Footer from "@/common/Footer.vue";

export default {
  name: "Home",
  components: {
    Hero,
    Brands,
    Features,
    Banner,
    Footer,
  },
};
</script>
