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
#app{
  height: 100%;
}
body{
  height: 100%;
}
html{
  height: 100%;
}
</style>
