<script setup>
import { ref } from 'vue' // necessário para reatividade

let isLoading = ref(false)
let isDisable = ref(false)
let isAble = ref(true)

function atualizarLoading() {
  isLoading.value = !isLoading.value
}

function atualizarDisable() {
  isDisable.value = !isDisable.value
}

function atualizarAble() {
  isAble.value = !isAble.value
}
</script>

<template>
<button :class="[
  isLoading ? 'loading' : '',
  isDisable ? 'disable' : '',
  isAble ? 'able' : ''
]">
  Utilizando a diretiva class
</button>

<button @click="atualizarLoading">Atualizar Loading</button>
<button @click="atualizarDisable">Atualizar Disable</button>
<button @click="atualizarAble">Atualizar Able</button>
</template>



<style scoped>
.able{
    color: green
}

.disable{
    color:red
}

.loading{
    color:yellow
}
</style>