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
            <div id="app">	
              <p>{{myStr}}</p>
              <p>{{myStr2}}</p>
              <button @click="myFunction()">Click Me</button>
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
  

  
  data() { 
    return{
      myStr: "Hello World!",
      myStr2:"",
      inputData:""
    }
  },
  methods:{
    myFunction: function () {	
      this.myStr2 = this.myStr.toLowerCase();
    }
  }

};
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
  gap:0.5rem;
  color:gray;
}
.buttons {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.clear {
  border: solid 1px var(--red);
  background-color: var(--red);
  color: white;
  padding: 1rem 0;
  border-radius: 20px;
  font-size: 16px;
  cursor: pointer;
  transition: 0.4s;
  width: 100%;
}
.clear:hover {
  background-color: white;
  color: var(--red);
}
.actionButtons {
  padding-top: 0.5rem;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
}
.encrypt {
  border: solid 1px var(--darkBlue);
  background-color: var(--darkBlue);
  color: white;
  padding: 1.3rem 0;
  border-radius: 24px;
  font-size: 16px;
  margin: 0 1rem 0 0;
  cursor: pointer;
  transition: 0.4s;
  width: 50%;
}
.encrypt:hover {
  background-color: white;
  color: var(--darkBlue);
}
.decrypt {
  border: solid 1px var(--grey);
  background-color: var(--mediumBlue);
  color: var(--grey);
  padding: 1.3rem 0;
  border-radius: 24px;
  font-size: 16px;
  cursor: pointer;
  transition: 0.4s;
  width: 50%;
}
.decrypt:hover {
  background-color: var(--grey);
  color: white;
}
</style>
