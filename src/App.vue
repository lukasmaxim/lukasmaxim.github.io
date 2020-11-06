<template>
  <div id="app">
    <Main/>
  </div>
</template>

<script>
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    Main
  }
}
</script>

<style>
* {
  background-color: #0D0F11;
}
#app {
  font-family: 'Archivo-Bold', Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #FFFFFF;
  margin-top: 60px;
}
@font-face {
    font-family: 'Archivo-Bold';
    src:url('./assets/fonts/Archivo-Bold.ttf.woff') format('woff'),
        url('./assets/fonts/Archivo-Bold.ttf.svg#Archivo-Bold') format('svg'),
        url('./assets/fonts/Archivo-Bold.ttf.eot'),
        url('./assets/fonts/Archivo-Bold.ttf.eot?#iefix') format('embedded-opentype'); 
    font-weight: normal;
    font-style: normal;
}

</style>
