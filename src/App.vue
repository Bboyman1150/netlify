<template>
  <div id="app">
    <Nav></Nav>
    <img alt="Vue logo" src="./assets/logo.png">
    <Movies></Movies>
   
  </div>
</template>

<script>
import Nav from './components/Nav.vue'
import Movies from './components/Movies.vue'

export default {
  name: 'App',
  components: {
   Nav,
   Movies
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
 
}
</style>
