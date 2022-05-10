<template>
  <div class="hello">
    <div class="logo">
      <img alt="Vue logo" src="../assets/logo.png">
    </div>
    <div class="inputText">
      <h1>jiji</h1>
    </div>
    <div class="outputText">
      <img src="../assets/doll.png" alt="doll image">
    </div>
  </div>

</template>

<script>
export default {
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .hello{
    display: flex;
    position: fixed;
    margin:2rem;
    height:100vh;
    background-color: var(--background);
  
  }
  /* Vector */
  .logo{
    padding-top: 2rem;
    
    /* Dark blue/dark-blue-300 */
    /* background: #0A3871; */
  }
  .outputText{
    /* Rectangle 1 */

position: absolute;
width: 400px;
height: 90vh;
left: 800px;
top:0;

/* White */
background: #FFFFFF;
/* shadow */
box-shadow: 0px 24px 32px -8px rgba(0, 0, 0, 0.08);
border-radius: 32px;
  }
</style>
