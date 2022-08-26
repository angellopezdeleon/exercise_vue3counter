<script>
  export default {
    data: () => ({
      contador: 0,
    }),

  methods: {
    incrementar() {
      this.contador++;
    },
    disminuir() {
      this.contador--;
    },
    reiniciar() {
      this.contador = 0;
    },
  },
}
</script>


<template>
<div class="container">
    <img src="./assets/logo.svg" alt="logoVue" width="125" height="125">
    <small>
      <h1>Hola mundo desde Vue</h1>
    </small>
    <hr />

    <h2>Contador: {{ contador }}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="disminuir()">-1</button>
    <button @click="reiniciar()">Reset</button>
  </div>
</template>


<style scoped>
.container{
  text-align: center;
}

small {
  color: crimson;
}

h1 {
  font: bolder;
}

h2{
  font-size: 2.5rem;
}

button{
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
}
</style>