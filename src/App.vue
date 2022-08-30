<template>
  <div>
    <div>
      <!-- <Navbar /> -->
      <!-- <Header title="adVANture" /> -->
      <Header />
      <Navbar />
    </div>
    <About title="Welcome!" />
    <Gallery />
    <Swiper />
    <Available />
    <Services />
    <CTA />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import About from "./components/About.vue";
import Navbar from "./components/Navbar.vue";
import Gallery from "./components/Gallery.vue";
import Swiper from "./components/Swiper.vue";
import Available from "./components/Available.vue";
import Services from "./components/Services.vue";
import CTA from "./components/CTA.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Header,
    About,
    Gallery,
    Swiper,
    Available,
    Services,
    CTA,
    Footer,
  },
};
</script>

<style scoped>
div {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>