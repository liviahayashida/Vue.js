<template>
  <button>
    <ButtonComponent>
      <h1>Hello World! (exemplo de texto)</h1>
    </ButtonComponent>
    <!-- slot recebe seu conteúdo -->
  </button>
</template>

<script>
import ButtonComponent from './ButtonComponent.vue';
export default {
  components: {
    ButtonComponent
  }
}
</script>
