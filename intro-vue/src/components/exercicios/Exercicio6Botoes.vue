<script setup>
let isLoading = false
let isDisable = false
let isAble = true
</script>


<template>
<h1>Botões de Estado</h1>
<button :class="[
  isLoading ? 'loading' : '',
  isDisable ? 'disable' : '',
  isAble ? 'able' : ''
]">
  Utilizando a diretiva class
</button>

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