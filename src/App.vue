<template>
  <div id="app">
    <home/>
  </div>
</template>

<script>
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style lang="scss">

$font-dir: "assets/fonts/Courgette/";
@font-face {
  font-family: 'Courgette';
  src: url($font-dir+'Courgette-regular.eot'), /* IE9 Compat Modes */
       url($font-dir+'Courgette-Regular.woff') format('woff'), /* Modern Browsers */
       url($font-dir+'Courgette-Regular.ttf')  format('truetype'), /* Safari, Android, iOS */
}

#app{
  height: 100%;
}
body{
  height: 100%;
  margin: 0px;
}
html{
  height: 100%;
}
</style>
