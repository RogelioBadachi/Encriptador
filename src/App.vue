<template>
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
html {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background:#E5E5E5;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
/* text-align: center;*/
  color: #2c3e50; 
  

  
}
</style>
