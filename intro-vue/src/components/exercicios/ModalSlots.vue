<template>
  <div class="modalslots">
    <slot name="header"></slot>
    <slot>Conteúdo padrão do modal (default)</slot>
    <slot name="footer"></slot>
  </div>
</template>

<script>
export default {
  name: 'ModalSlots'
}
</script>

<style scoped>
* {
  background-color: #39cee4;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  font-size: 16px;
}
</style>
