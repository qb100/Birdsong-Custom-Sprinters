<template>
  <div class="top">
    <h3><span>&#xA9;</span>2022 adVANture LLC. All rights reserved</h3>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
* {
  background-color: hsl(34, 44%, 69%);
  color: black;
  padding-top: 2rem;
  display: flex;
  align-items: center;
}

h3 {
  display: flex;
  justify-content: center;
  align-items: flex-end;
  padding-top: 2rem;
  font-size: 1rem;
  position: absolute;
  max-height: 0.25rem;
}

span {
  padding-right: 0.5rem;
}
</style>