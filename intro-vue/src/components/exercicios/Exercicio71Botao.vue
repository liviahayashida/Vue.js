<script setup>
import { ref } from 'vue' // necessário para reatividade

let isLoading = ref(false)
let isDisable = ref(false)
let isAble = ref(false)
const contador = ref(0)
const estado = ref('ativo')

function incrementar (){
    contador.value++
}

functiondecrementar(){
    if (contador > 0){
        contador.value--
    }
}

function resetar(){
    contador.value = 0
}

function alterarEstado(){

}
</script>

<template>
    <div>
        <p>contador: {{  contador }}</p>
        <p>estado : {{  estado }}</p>
        <button @click="decrementar": disable="contador ===0"></button>
    </div>
<button :class="[
  isLoading ? 'loading' : '',
  isDisable ? 'disable' : '',
  isAble ? 'able' : ''
]">
  Utilizando a diretiva class
</button>
<h1> Contando : $contador</h1>
<button @click="atualizarLoading">Atualizar Loading (0)</button> 
<button @click="atualizarDisable">Atualizar Disable (-1)</button>
<button @click="atualizarAble">Atualizar Able (+1)</button>
</template>



<style scoped>
.atualizarAble{
    color: green
}

.atualizarDisable{
    color:red
}

.atualizarLoading{
    color:yellow
}
</style>