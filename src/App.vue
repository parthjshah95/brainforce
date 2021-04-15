<template>
  <div id="app">
    <div class="title-bar">
      <div>
        <span class="title">
          BrainForce
        </span>
        <span class="subtitle">Take control!</span>
      </div>
      <div>
        <span>
          <!-- <router-link to="/">Home</router-link>
          <router-link to="/">Team</router-link> -->
        </span>
      </div>    
    </div>
    <!-- <home/> -->
    <!-- <router-link to="/">Home</router-link> -->
    <router-view/>
  </div>
</template>

<script>
import Home from '@/views/Home.vue'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style lang="scss">

$title-bar-padding: 15px;
$title-font-size: 40px;
$box-shadow: 0 5px 20px rgba(0,0,0,0.19), 0 3px 6px rgba(0,0,0,0.23);
$box-shadow-highlight: 0 5px 30px rgba(0,0,0,0.19), 0 3px 15px rgba(0,0,0,0.23);
$content-padding: 40px;
$orange: #f46524;


$font-dir: "assets/fonts/Courgette/";
@font-face {
  font-family: 'Courgette';
  src: url($font-dir+'Courgette-Regular.eot'), /* IE9 Compat Modes */
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
.flex-container{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-evenly;
}
.title-bar{
  @extend .flex-container;
  justify-content: space-between;
  width: 100%;
  padding: $title-bar-padding;
  background-color: $orange;
  color: white;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 100;
}
.title{
  font-family: 'Lobster', cursive;
  font-size: $title-font-size;
}
.subtitle{
  font-style: italic;
  font-family: Courgette;
}
</style>
