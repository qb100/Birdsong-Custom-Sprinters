<template>
  <div>
    <h2 id="services" class="heading">Services We Offer:</h2>
    <p class="heading-info">
      Want to outfit your rig into your dream, off-roading machine? We can help!
      Check out our services below!
    </p>
    <div class="services-grid">
      <div>
        <img
          src="../assets/img/backwoods.jpg"
          alt="bumper modification"
        /><br />
        <a
          href="https://backwoodsadventuremods.com/"
          target="_blank"
          rel="noopener noreferrer"
          >Backwoods Adventure Mods</a
        >
        <p>
          Makers of the best roof racks, bumpers, box carriers, lights and so
          much more.
        </p>
      </div>
      <div>
        <img src="../assets/img/snorkel.jpg" alt="snorkel mod on van" /><br />
        <a
          href="https://www.terrawagen.com/"
          target="_blank"
          rel="noopener noreferrer"
          >Terrawagen Snorkels</a
        >
        <p>
          Not just for diving in deep, they're great for circulating clean air
          when off road.
        </p>
      </div>
      <div>
        <img
          src="../assets/img/flares.jpg"
          alt="interior view of a window flare"
        /><br />
        <a
          href="https://flarespace.com/"
          target="_blank"
          rel="noopener noreferrer"
          >Flare by FlareSpace</a
        >
        <p>
          Flares can help make a van feel spacious. They're also great for a
          little bit of extra room, a wall-to-wall bed frame or an extra window.
        </p>
      </div>
      <div>
        <img src="../assets/img/windows.jpg" alt="bumper modification" /><br />
        <a
          href="https://vanwindowsdirect.com/"
          target="_blank"
          rel="noopener noreferrer"
          >Window Installs</a
        >
        <p>Add light, circulate air and vent while cooking.</p>
      </div>
    </div>
    <div>
      <p class="list-head">Other services we offer:</p>
      <ul class="list">
        <li>Fan Installs</li>
        <li>Insulation</li>
        <li>Water Tanks and/or Water Pumps</li>
        <li>Walls and/or Ceilings</li>
        <li>Ladders</li>
        <li>Electric/Batteries</li>
        <li>Diesel Heaters</li>
        <li>Cabinets</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Services",
};
</script>

<style scoped>
* {
  /* font-family: "Clash Grotesk", sans-serif; */
  padding-top: 1rem;
  max-width: 80%;
  margin-right: auto;
  margin-left: auto;
}

.heading {
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: "Panchang", sans-serif;
}

.heading-info {
  display: flex;
  justify-content: center;
  align-items: center;
}

.services-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
}

@media (max-width: 900px) {
  .services-grid {
    display: flex;
    flex-direction: column;
  }
}

img,
a {
  display: flex;
  justify-content: center;
}

.list-head {
  display: flex;
  justify-content: center;
  padding-bottom: 0;
  font-family: "Panchang", sans-serif;
}

.list {
  display: grid;
  grid-template-columns: 1fr 1fr;
  padding-top: 0;
}

@media (max-width: 900px) {
  .list {
    display: flex;
    flex-direction: column;
  }
}

li {
  width: 100%;
  padding-top: 0.5rem;
}

.heading-info,
p,
li {
  font-family: "Satoshi", sans-serif;
}
</style>