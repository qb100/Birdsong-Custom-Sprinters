<template>
  <div class="nav">
    <div class="nav-container">
      <div class="comp">
        <h3>adVANture</h3>
      </div>
      <div class="links">
        <h3><a href="#about">About Us</a></h3>
        <h3><a href="#gallery">Gallery</a></h3>
        <h3><a href="#available">Available Vans</a></h3>
        <h3><a href="#services">Services</a></h3>
        <h3><a href="#contact">Contact Us</a></h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
.nav-container {
  display: grid;
  grid-template-columns: 1fr 50%;
  width: 80%;
  margin-left: auto;
  margin-right: auto;
}

.comp {
  color: hsl(34, 44%, 71%);
  font-size: 1rem;
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
  font-family: "Clash Grotesk", sans-serif;
}

@media (max-width: 900px) {
  .comp {
    visibility: hidden;
  }
}

.links {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

@media (max-width: 1020px) {
  .links {
    display: block;
    visibility: visible;
  }
}

a {
  cursor: alias;
  text-decoration: none;
  color: hsl(0, 0%, 0%);
  font-family: "Satoshi", sans-serif;
}

a:hover {
  text-decoration: underline;
  color: rgb(0 0 255);
}
</style>