<template>
  <button class="buttoncomponent">
    <slot />
  </button>
</template>

<script>
export default {
  name: 'ButtonComponent'
}
</script>

<style scoped>

*{
    background-color: #b53054;
    color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  font-size: 16px;
}
</style>