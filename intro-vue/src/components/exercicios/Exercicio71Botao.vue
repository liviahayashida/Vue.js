<script setup>
import { ref } from 'vue' // necessário para reatividade

const isLoading = ref(false)
const isDisable = ref(false)
const isAble = ref(false)
const contador = ref(0)
const estado = ref('ativo')

function incrementar (){
    contador.value++
}


function decrementar() {
    if (contador.value > 0) {
        contador.value--;
    }
}

function resetar(){
    contador.value = 0
}


function atualizarLoading() {
    isLoading.value = !isLoading.value;
}
function atualizarDisable() {
    isDisable.value = !isDisable.value;
}
function atualizarAble() {
    isAble.value = !isAble.value;
}
</script>

<template>
    <div>
    <p>contador: {{ contador }}</p>
        <p>estado : {{  estado }}</p>
    <button @click="decrementar" :disabled="contador === 0">-</button>
    </div>
<button :class="[
    isLoading ? 'atualizarLoading' : '',
    isDisable ? 'atualizarDisable' : '',
    isAble ? 'atualizarAble' : ''
]">
    Utilizando a diretiva class
</button>
<h1> Contando : {{ contador }}</h1>
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