<template>
  <swiper
    :rewind="true"
    :navigation="true"
    :modules="modules"
    class="mySwiper"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
  >
    <swiper-slide
      ><img
        class="bertha"
        src="../assets/img/Bertha-driver.jpg" /></swiper-slide
    ><swiper-slide
      ><img class="bertha-s" src="../assets/img/Big-Bertha-side.jpg"
    /></swiper-slide>
    <swiper-slide
      ><img class="gina" src="../assets/img/Gina-front.jpg" /></swiper-slide
    ><swiper-slide
      ><img class="van-diesel" src="../assets/img/Van-Diesel.jpg"
    /></swiper-slide>
    <swiper-slide
      ><img class="window" src="../assets/img/b-window.jpg" /></swiper-slide
    ><swiper-slide
      ><img class="corner" src="../assets/img/back-corner.jpg" /></swiper-slide
    ><swiper-slide
      ><img class="tray" src="../assets/img/bike-tray.jpg" /></swiper-slide
    ><swiper-slide
      ><img class="rack" src="../assets/img/roof-rack.jpg"
    /></swiper-slide>
  </swiper>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";

import "swiper/css";

//import "./style.css";

import "swiper/css/navigation";

import { Navigation } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Navigation],
    };
  },
};
</script>

<style scoped>
body {
  background: #eee;
  color: #000;
}

.swiper {
  max-width: 35rem;
}

@media (max-width: 900px) {
  .swiper {
    max-width: 90%;
  }
}

.swiper-slide {
  background: hsl(34, 44%, 69%);

  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  /* -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center; */
  justify-content: center;
  /* -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center; */
  align-items: center;
  max-width: 100%;
  height: auto;
}

.swiper-slide img {
  display: block;
  width: 75%;
  /* height: 30%; */
  object-fit: cover;
}
</style>