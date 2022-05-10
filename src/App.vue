<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <EncriptadorVue />
</template>

<script>
import EncriptadorVue from './components/encriptadorVue.vue'

export default {
  name: 'App',
  components: {
    EncriptadorVue
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
