<template>
  <div id="about" class="container">
    <div class="intro">
      <h2>Welcome!</h2>
      <p>
        Hello! We're Brandon and Brittni, owners and outfitters of adVANture
        LLC. We spent three amazing years living out of a variety of Mercedes
        Sprinter vans that we designed and outfitted! Each van has brought us so
        much happiness and unforgettable memories. In the beginning, we wanted
        to get out of debt, stop living for the weekend and train in the most
        conducive places while building up to the 2020 Olympic Marathon Trials.
        Fast forward, we received so much interest in our rigs that it blossomed
        into a small, van outfitting business! Today, we're rooted in Alamosa,
        Colorado where we can invest our hearts and imaginations into every
        build. Check out our rigs below and thanks for stopping by!<br /><span
          >Cheers! B & B</span
        >
      </p>
    </div>
    <div class="profile-img">
      <img
        class="profile-pic"
        src="https://static.wixstatic.com/media/4724ae_275cfa9da1554242858eaeab52ad3281~mv2.jpg/v1/fill/w_980,h_736,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/17885168912083390.jpg"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<style scoped>
.container {
  display: grid;
  grid-template-columns: 60% auto;
  background-color: hsl(34, 44%, 71%);
  margin-top: 2rem;
  width: 80%;
  margin-left: auto;
  margin-right: auto;
}

@media (max-width: 900px) {
  .container {
    display: flex;
    flex-direction: column;
    width: 90%;
  }
}

h2 {
  font-size: 2rem;
  display: flex;
  justify-content: center;
  font-family: "Panchang", sans-serif;
}

p {
  font-size: 1.25rem;
  padding-left: 0.75rem;
  padding-right: 0.75rem;
  font-family: "Satoshi", sans-serif;
}

span {
  display: flex;
  justify-content: center;
  padding-top: 1rem;
}

.profile-img {
  display: flex;
  justify-content: center;
  align-items: center;
}

.profile-pic {
  padding-left: 20%;
  width: 100%;
}

@media (max-width: 900px) {
  .profile-pic {
    padding-left: 0;
    width: 90%;
  }
}
</style>