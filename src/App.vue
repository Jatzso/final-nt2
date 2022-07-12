<template>
  <div id="app">
    <Funcionalidad />
  </div>
</template>

<script>
import Funcionalidad from './components/Funcionalidad.vue'
export default {
  name: 'App',
  components: {
   Funcionalidad
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
  margin-top: 60px;
}
</style>
