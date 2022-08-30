<template>
  <div id="contact" class="split">
    <div class="contact">
      <h2>Contact Us:</h2>
      <h4>Alamosa, Colorado</h4>
      <h4>
        Brandon:
        <a
          href="mailto:brandon@runyourpersonalbest.com"
          target="_blank"
          rel="noopener"
          >brandon@runyourpersonalbest.com</a
        >
      </h4>
      <h4>
        Brittni:
        <a href="mailto:brittni.hutton@gmail.com" target="_blank" rel="noopener"
          >brittni.hutton@gmail.com</a
        >
      </h4>
      <h4>We look forward to hearing from you.</h4>
    </div>
    <div class="sunset">
      <img
        class="sunset-img"
        src="../assets/img/sunset.jpg"
        alt="camp chairs by van at sunset"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "CTA",
};
</script>

<style scoped>
* {
  /* font-family: "Clash Grotesk", sans-serif; */
  background-color: hsl(34, 44%, 71%);
  margin-top: 1rem;
  width: 80%;
  margin-right: auto;
  margin-left: auto;
}

h2 {
  font-family: "Panchang", sans-serif;
}

h4 {
  font-family: "Satoshi", sans-serif;
}

@media (max-width: 900px) {
  h4 {
    font-size: 0.9rem;
  }
}

.split {
  display: grid;
  grid-template-columns: 70% auto;
}

@media (max-width: 900px) {
  .split {
    display: flex;
  }
}

.contact {
  /* border: 2px solid red; */
  display: block;
  width: 100%;
}

.sunset {
  display: flex;
  justify-content: center;
  align-items: center;
}

.sunset-img {
  display: flex;
  justify-content: center;
  align-items: center;
  object-fit: fill;
  width: 100%;
  height: auto;
  padding-bottom: 1rem;
}
</style>>