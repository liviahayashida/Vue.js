<script setup>
let validacao = false
let isError = false
let isActive = true
let isDisable = false
</script>


<template>
<!-- <p :class="validacao ? 'ok' : 'falha'"> Utilizando a diretiva class</p> -->

<p clas="{
'ok' : isActive,
'falha' : isError
}">Teste Diretiva Class</p>

<button :disable="isDisable">Clique aqui</button>
</template>

<style scoped>
.ok{
    color: green
}

.falha{
    color:red
}
</style>