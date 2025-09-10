<template>
  <div>
    <Card>
      <h1>Hello World!</h1>
      <p>Este é um parágrafo de exemplo.</p>
    </Card>
    <!-- slot recebe seu conteúdo -->
    
    <Card>
      <img src="https://via.placeholder.com/150" alt="Imagem de exemplo">
    </Card>
  </div>
</template>

<script>
import Card from '../../Card.vue';
export default {
  components: {
    Card
  }
}
</script>

<!-- <template>
  <div> <!-- This div makes the card-like appearance -->
    <!-- <slot>EXEMPLO DE SLOTS</slot>
  </div> -->
<!-- </template>

<script></script>

<style scoped>
  div {
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    border-radius: 10px;
    margin: 10px;
  }
</style> --> 