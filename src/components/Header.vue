<template>
  <header>
    <video width="320" height="240" autoplay loop muted>
      <source src="../assets/video/van-video.mp4" type="video/mp4" />
    </video>

    <div>
      <!-- <h1>{{ title }}</h1> -->
      <h1>ad<span>VAN</span>ture</h1>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    title: String,
  },
};
</script>

<style scoped>
header {
  position: relative;
  border: 2px solid black;
}

span {
  color: hsl(34, 44%, 69%);
}

video {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: -5;
  opacity: 0.5;
}

h1 {
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 4rem;
  letter-spacing: 0.25rem;
  font-family: "Panchang", sans-serif;
  padding-top: 7rem;
  padding-bottom: 7rem;
}

@media (max-width: 900px) {
  h1 {
    font-size: 2rem;
  }
}
</style>