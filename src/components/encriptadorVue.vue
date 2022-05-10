<template>
  <div class="hello">
    <div class="clark">
      <div class="logo">
        <img alt="Vue logo" src="../assets/logo.png">
      </div>
      <div class="inputText">
        <textarea
            class="textarea"
            v-model="inputData"
            placeholder="Ingrese el texto aquí"
            required
          ></textarea>
        <div class="send">
          <div class="btnMessage">
            <i class="fa-solid fa-circle-exclamation"></i>
            <p>Sólo letras minúsculas y sin acentos</p>
          </div>
        </div>
        <div class="buttons">
            <button @click="clearData" class="clear">Limpiar</button>
            <div class="actionButtons">
              <button class="encrypt" @click="encryptData">Encriptar</button>
              <button class="decrypt" @click="decryptData">Desencriptar</button>
            </div>
          </div>  
      </div> <!--Aqui termina inputText-->
    </div>
    <div class="whiteBox">
      <div class="outputText">
        <img src="../assets/doll.png" alt="doll image">
        <h2>Ningún mensaje fue encontrado</h2>
        <h3>Ingresa el texto que deseas Encriptar o Desencriptar</h3>
      </div>
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

position: relative;
width: 400px;
height: 90vh;
top:0;

/* White */
background: #FFFFFF;
/* shadow */
box-shadow: 0px 24px 32px -8px rgba(0, 0, 0, 0.08);
border-radius: 32px;
  }
  .whiteBox{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 25vw;
  }
  .textarea {
  height: 300px;
  width: calc(100% - 30px);
  background-color: transparent;
  border: none;
  resize: none;
  outline: none;
  text-align: center;
  font-size: 32px;
  color: var(--darkBlue);
}
.clark{
  width: 70vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
}
.btnMessage{
  display: flex;
  flex-direction: row;
  align-items: center;
}
</style>
