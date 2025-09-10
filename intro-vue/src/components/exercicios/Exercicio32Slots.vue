<template>
  <ModalSlots>
    <template v-slot:header>
      <h1>Hello World! (exemplo de header)</h1>
    </template>

    <template v-slot:default>
    </template>

    <template v-slot:footer>
      <p>Exemplo de footer</p>
    </template>
  </ModalSlots>
</template>

<script>
import ModalSlots from './ModalSlots.vue';

export default {
  components: {
    ModalSlots
  }
}
</script>