<template>
  <div id="app">
    <Header/>
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style>
* {
  background-color: #FFF1DF;
}
#app {
  font-family: 'Lovelo', Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #444444;
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
@font-face {
    font-family: 'Lovelo';
    src: url('./assets/fonts/Lovelo_Black.ttf') format('truetype');
}

</style>
