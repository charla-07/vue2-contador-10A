<script>
  export default{
    data:() => ({
      contador:10,
    }),

    methods:{
      saludar(){
        console.log("Hola 10A | @")
      },
      incrementar() {
        this.contador++;
      },
      decrementar() {
        this.contador--;
      },
      resetear(){
        this.contador = 10;
      }
    }
  };
</script>

<template> 
  <div class="container-fluid">
    <div class="alert alert-secondary" role="alert" style="padding: 10px 130px !important; margin-top: 20px;">
      Karla Elena Francisco Manuel 10A DGS
    </div>
  </div>
  <img src="./assets/logo.svg" alt="Logo VUE" width="125" height="125">
  <div class="container">
    <small>
      <h1>Hola desde VUE.js 3</h1>
    </small>
    <hr>
    <h2>Contador {{contador}}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="decrementar()">-1</button>
    <button @click="resetear()">Reset</button>
  </div>
</template>

<style scoped>
  .container{
    text-align: center;
  }
  h1 {
    font-weight: bolder;
  }
  h2{
    font-size: 2.5rem;
  }
  small{
    color:#666;
  }
  button {
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 8px;
  }
</style>