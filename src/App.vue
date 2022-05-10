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
:root{
    --lightBlue: #f3f5fc;
  --mediumBlue: #d8dfe8;
  --darkBlue: #0a3871;
  --lightGrey: #d8dfe8;
  --grey: #495057;
  --darkGrey: #343a40;
  --red: rgb(182, 65, 65);
}
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
