<script setup>
let usuariologado = true
import { ref } from 'vue' // improtando para que se torne reativa
function Logar() { usuariologado.value = !usuariologado.value; } //função
</script>

<template>
<button @click="Logar"> Fazer Log In
  </button>
      <h1 v-if='usuariologado'>Bem vindo!</h1>
<h1 v-else>Não logado</h1>
</template> 