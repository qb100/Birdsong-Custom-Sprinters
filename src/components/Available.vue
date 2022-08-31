<template>
  <h2 id="available" class="available">Available Vans</h2>

  <div class="columns">
    <div class="van">
      <div class="van-info">
        <h2 class="name">Van Diesel</h2>
        <h3>2020 Mercedes Sprinter 170"</h3>
        <h4>
          4x4<br />High Roof<br />Odo: 18,700<br />Diesel<br />Price: $175,999
        </h4>
        <p>
          This van is about functionality! Van Diesel has a comfortable set up
          with a massive bed, a custom made live edge bench seat and lots of
          storage. Check out the details and photos below!
        </p>
        <div>
          <button :class="{ active: isActive }" @click="toggle = !toggle">
            {{ text }}
          </button>
          <div v-show="toggle">
            <h5>Exterior Mods:</h5>
            <p class="exterior-mods">
              - Backwoods Adventure Mods Front/Rear Bumper <br />
              - Owl Vans swing-arm ladder and tire carrier <br />
              - Backwoods roof rack <br />
              - Van Compass Stage 3 suspension / lift kit: Falcon 2.1 shocks and
              mounting system, 4x4 sprinter sumo rings, rear falcon 2.1 shocks,
              rear mini pack and upgraded leaf springs, and dust boots for all 4
              shocks.<br />
              - Van compass floating light mounts<br />
              - Warn VR xenon 12-s winch<br />
              - 16 in Black Rhino wheels x 5<br />
              - BFG KO2 265/75/r16 Tires x 5<br />
              - 2 x 9" Pathfinder prowler driving lights<br />
              - Rear back-up pathfinder recessed lights<br />
              - 50" pathfinder recessed light bar on roof rack<br />
              - Front pathfinder surface mount pod flood lights<br />
              - Front pathfinder surface mount pods spot lights<br />
            </p>
            <h5>Interior Mods:</h5>
            <p class="interior-mods">
              - Custom wrapped birch walls and ceilings<br />
              - Pine tongue and groove ceiling<br />
              - Durable marine flooring<br />
              - Lost Hiway powder Coated aluminum kitchen galley w/ slides for
              fridge<br />
              - Lost Hiway powder Coated aluminum small faucet/sink galley<br />
              - Lost Hiway powder Coated aluminum bench seat w/ 500lb slide w/
              toilet<br />
              - Butcher block counter top<br />
              - 6 x powder coated upper cabinets w/ birch soft closing doors<br />
              - Lost Hiway bed (78" x 68" w/ hidden storage big enough for skis,
              poles, valuables, and whatever you fancy.<br />
              - Lost Hiway passenger's side fender storage box: powder coated
              aluminum w/ door to hide controls and access panel for
              water/pump.<br />
              - Lost Hiway driver's side fender storage box: powder coated
              aluminum w/ 3 storage drawers and access panel for electric and
              storage.<br />
              Quick disconnect shower head - Custom Aluminum bed-frame<br />
              - Custom Tochta mattress w/ hinge for access to hidden storage<br />
              - Custom bench seat/storage with live edge elm and pine tongue and
              groove<br />
            </p>
            <h5>Electric:</h5>
            <p class="electric">
              - Renogy 200 AH Smart lithium batteries<br />
              - Renogy smart battery to battery (alternator) charger<br />
              - Renogy smart solar charger<br />
              - 200 watts of Renogy Solar Panels<br />
              - Renogy smart bluetooth module to access battery info via app<br />
              - Renogy 2000 watt inverter/charger<br />
              - Blue Sea main on/off switch<br />
              - 2 x 110 recessed outlets<br />
              - 2 x usb charger (not including front cabin chargers)<br />
              - 9 x recessed puck lights (on different dimmable switches)<br />
              - Reading light above bed<br />
              - Dimmable puck light above kitchen galley<br />
            </p>
            <h5>Appliances:</h5>
            <p class="appliances">
              - Dometic Fridge/freezer combo<br />
              - Stainless steel deep sink<br />
              - Rear shower w/ electric surflo pump and strainer. Also great for
              cleaning your bike<br />
              - 20 gallon fender box tank for quick disconnect shower<br />
            </p>
            <h5>Climate Control:</h5>
            <p class="climate">
              - CR Laurence T-vent Window (sliding door)<br />
              - CR Laurence T-vent Window (behind driver's side)<br />
              - 2 x Maxxair fan (both ways)<br />
              - Espar d2s2 high altitude diesel heater with remote<br />
              - 3m and Wool insulation<br />
              - Adventure Van Co insulated magnetic curtains for stealth
              sleeping and climate control<br />
            </p>
          </div>
        </div>
      </div>
      <div class="van-pics">
        <swiper
          :style="{
            '--swiper-navigation-color': '#fff',
            '--swiper-pagination-color': '#fff',
          }"
          :loop="true"
          :spaceBetween="10"
          :navigation="true"
          :modules="modules"
          class="mySwiper2"
          @swiper="onSwiper"
          @slideChange="onSlideChange"
        >
          <swiper-slide
            ><img src="../assets/img/Van-Diesel.jpg"
          /></swiper-slide>
          <swiper-slide><img src="../assets/img/diesel-1.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/diesel-2.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/diesel-3.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/diesel-4.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/diesel-5.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/diesel-6.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/diesel-7.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/diesel-8.jpg" /></swiper-slide>
        </swiper>
      </div>
    </div>
    <br />
    <div class="van">
      <div class="van-info">
        <h2 class="name">Gina</h2>
        <h3>2021 Mercedes Sprinter 144"</h3>
        <h4>
          4x4<br />High Roof<br />Odo: 1500<br />Diesel<br />Price: $175,999
        </h4>
        <p>
          Gina is one of our "fanciest" builds! She has custom cabinets, a
          one-of a kind mountain backsplash, and lights for any occasion. We
          love her good-vibes! Check out the details and photos below!
        </p>
        <div>
          <button @click="toggleTwo = !toggleTwo">{{ text }}</button>
          <div v-show="toggleTwo">
            <h5>Exterior Mods:</h5>
            <p>
              - Van Compass front bumper w/ recessed winch mount<br />
              - Van Compass floating light mount<br />
              - Backwoods Adventure Mods roof rack<br />
              - Backwoods Adventure Mods side ladder<br />
              - Van Compass Stage 3 suspension / lift kit: Falcon 2.1 shocks and
              mounting system, 4x4 sprinter sumo rings, rear falcon 2.1 shocks,
              rear mini pack and upgraded leaf springs, and dust boots for all 4
              shocks.<br />
              - Warn VR evo 10-s winch<br />
              - Rhino Lined Flare-space flares - allows you to sleep sideways
              (79 inches) and frees up more space inside<br />
              - 16in Black Rhino wheels x 5<br />
              - BFG KO2 Tires (265/75r16) x 5<br />
              - 50" Pathfinder recessed light bar on roof rack<br />
              - 2 x 9" Pathfinder prowler driving lights<br />
            </p>
            <h5>Interior Mods:</h5>
            <p>
              - 1/4' birch wrapped in insulated foam and fire retardant
              fabric<br />
              - Durable Lonseal marine coin floor<br />
              - Custom CNC'd baltic birch with laminate overlay for
              protection<br />
              - Kitchen galley w/ plenty of storage<br />
              - Acacia butcher block counter top<br />
              - Custom stainless steel backsplash with powder coated aluminum
              mountain range<br />
              - 5 x upper cabinets w/ soft closing hinges w/ 1 x rear cubby<br />
              - Driver's side storage fender/electrical storage box w/ 3 x doors
              to hide controls and access panel for electric<br />
              - Passenger's side fender storage box: hides 20 gallon water tank
              w/ plenty of storage<br />
              - Space saving flare trim rings<br />
              - Custom Aluminum bed-frame<br />
              - Custom Tochta mattress<br />
              - 2 x bench seats w/ a massive amount of storage<br />
              - Rear door storage cubbies<br />
              - Reliance toilet<br />
            </p>
            <h5>Electric:</h5>
            <p>
              - Renogy 200 AH Smart lithium "self heating" batteries, perfect
              for winter<br />
              - Renogy smart DC to DC (alternator) charge<br />
              - Renogy smart solar charger<br />
              - 200 watts of Renogy Solar Panels<br />
              - Renogy smart bluetooth module to access battery info via app<br />
              - Renogy 2000 watt inverter<br />
              - Blue sea main on/off switch<br />
              - 2 x touch (dimmable) reading lights in flare trim ring<br />
              - 2 x 110 recessed outlets w/ usb charging<br />
              - 4 x usb charger (not including front cabin chargers)<br />
              - 6 x recessed puck lights (on a dimmable touch switch)<br />
              - Recessed rope light underneath cabinets (on a dimmable touch
              switch) <br />
              - 20 gallon water tank / 7 gallon grey water tank (with option to
              dump straight onto the ground)<br />
            </p>
            <h5>Appliances:</h5>
            <p>
              - Isotherm cruise elegance 85 fridge<br />
              - Ramblewood 2 burner stovetop<br />
              - Stainless steel deep sink / faucet<br />
              - Rear shower w/ electric surflo pump and strainer<br />
              - 20 gallon fender box tank for quick disconnect shower<br />
            </p>
            <h5>Climate Control:</h5>
            <p>
              - CR Laurence T-vent Window (sliding door)<br />
              - Maxxair fan (both ways)<br />
              - Rear arctic term window<br />
              - Espar d2s2 high altitude diesel heater with remote<br />
              - 3m thinsulate / Havelock wool insulation<br />
              - Adventure Van Co insulated magnetic curtains for stealth
              sleeping and climate control<br />
              - Interior run plumbing<br />
            </p>
          </div>
        </div>
      </div>
      <div class="van-pics">
        <swiper
          :style="{
            '--swiper-navigation-color': '#fff',
            '--swiper-pagination-color': '#fff',
          }"
          :loop="true"
          :spaceBetween="10"
          :navigation="true"
          :modules="modules"
          class="mySwiper2"
          @swiper="onSwiper"
          @slideChange="onSlideChange"
        >
          <swiper-slide
            ><img src="../assets/img/Gina-front.jpg"
          /></swiper-slide>
          <swiper-slide><img src="../assets/img/gina-1.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/gina-2.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/gina-3.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/gina-4.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/gina-5.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/gina-6.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/gina-7.jpg" /></swiper-slide>
          <swiper-slide><img src="../assets/img/gina-8.jpg" /></swiper-slide>
        </swiper>
      </div>
    </div>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";

import "swiper/css";

import "swiper/css/free-mode";
import "swiper/css/navigation";
import "swiper/css/thumbs";

import { FreeMode, Navigation, Thumbs } from "swiper";
import About from "./About.vue";

export default {
  name: "Available",
  data() {
    return {
      toggle: false,
      toggleTwo: false,
      text: "More Info:",
    };
  },
  components: {
    Swiper,
    SwiperSlide,
    About,
  },
  setup() {
    return {
      modules: [FreeMode, Navigation],
    };
  },
};
</script>

<style scoped>
.available {
  display: flex;
  justify-content: center;
  align-items: center;
  padding-top: 3rem;
  font-family: "Panchang", sans-serif;
}

button {
  padding: 0.25rem 2rem;
  background-color: hsl(34, 44%, 69%);
}

.van {
  display: grid;
  grid-template-columns: 50% 100%;
  gap: 3rem;
  background-color: hsl(34, 44%, 71%);
  padding-left: 0.75rem;
  padding-bottom: 2rem;
  width: 80%;
  margin-right: auto;
  margin-left: auto;
  border-radius: 7px;
}

@media (max-width: 900px) {
  .van {
    display: flex;
    flex-direction: column;
  }
}

.name {
  padding-top: 2rem;
  font-family: "Panchang", sans-serif;
}

.van-pics {
  max-width: 50%;
  padding-top: 3rem;
}

h5 {
  font-size: 1rem;
}

h3,
h4,
h5,
p {
  font-family: "Satoshi", sans-serif;
}

.exterior-mods,
.interior-mods,
.electric,
.appliances,
.climate {
  line-height: 1.25rem;
}

.swiper-slide {
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

body {
  background: #000;
  color: #000;
}

.swiper {
  width: 100%;
  max-height: 30rem;
  margin-left: auto;
  margin-right: auto;
  border-radius: 8px;
}

.swiper-slide {
  background-size: cover;
  background-position: center;
}

.mySwiper2 {
  height: 100%;
  width: 100%;
}

.mySwiper {
  height: 30%;
  box-sizing: border-box;
  padding: 0.5rem 0;
}

.mySwiper .swiper-slide:hover {
  opacity: 1;
}

.mySwiper .swiper-slide {
  width: 25%;
  height: 100%;
  opacity: 0.7;
}

.mySwiper .swiper-slide-thumb-active {
  opacity: 1;
}
</style>