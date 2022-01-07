<template>
  <div id="container">
    <div id="photo-container">
      <!-- <img src="./src/assets/images/portrait.png"/> -->
    </div>
    <div id="text-container">
      Text
    </div>
  </div>
</template>

<script>
export default {
  name: "Landing"
};
</script>

<style scoped>
#container {
  height: 100%;
  display: grid;
  grid-template-columns: 0.3fr 1fr 1fr 1fr 0.3fr;
  grid-template: ". photo text text .";
}
#photo-container {
  grid-area: photo;
  background-color: blue;
}
#text-container {
  grid-area: text;
  background-color: orange;
}
</style>
