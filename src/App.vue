<template>
  <div id="app">
    <Header />
    <router-view></router-view>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer
  }
};
</script>

<style>
* {
  background-color: #fff1df;
}
#app {
  font-family: "Roboto Mono", Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #444444;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
html,
body {
  margin: 0 !important;
}
@font-face {
  font-family: "Lovelo";
  src: url("./assets/fonts/Lovelo_Black.ttf") format("truetype");
}
@import url("https://fonts.googleapis.com/css2?family=Roboto+Mono:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;1,100;1,200;1,300;1,400;1,500;1,600;1,700&display=swap");
router-link,
button {
  height: fit-content;
  width: fit-content;
  padding: 1em;
  border: 0.15em solid #393939;
  border-radius: 0.3em;
  cursor: pointer;
  font-family: "Roboto Mono"; /* why does app ruleset not apply here? */
  font-weight: 500;
  color: #393939;
}
a {
  font-weight: 900;
  color: #393939;
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
  color: #570d49;
}
</style>
