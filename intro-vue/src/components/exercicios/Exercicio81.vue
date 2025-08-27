<script setup>
import {ref} from 'vue'
let inputValue = ref('')

function mensagem(){
alert (`Executando a função Enter:  ${inputValue.value}`)
}

function aviso(){
alert (`Voce clicou na tecla na função Shift:  ${inputValue.value}`)
}

function alerta(){
alert (`Voce pressionou a função ?:  ${inputValue.value}`)
}
</script>

<template>

 <br><input type="text" @keyup.enter="mensagem" v-model="inputValue"></input>
<br><input type="text" @keydown.shift="aviso" v-model="inputValue"></input>
<br><input type="text" @keypress.?="alerta" v-model="inputValue"></input>

</template>