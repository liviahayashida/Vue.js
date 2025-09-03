<script setup>
import {ref} from 'vue'
const emit = defineEmits(['update'])
const count = ref(0)

function Increment (){
    count.value++
    emit('update', count.value)
}
</script>

<template>
 <div>
    <p>Contador: {{ count }}</p>
    <button @click="Increment"> +1</button>
 </div>
</template>