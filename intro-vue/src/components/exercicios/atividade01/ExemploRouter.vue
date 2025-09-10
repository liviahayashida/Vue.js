<template>
  <p>Choose what part of this page you want to see:</p>
  <button @click="activeComp = 'animal-collection'">Animals</button>
  <button @click="activeComp = 'food-items'">Food</button><br>
  <div>
    <router-view></router-view>
    <component :is="activeComp"></component>
  </div>
</template>
<script>
import { ref } from 'vue';

// Componentes fictícios para exemplo
const AnimalCollection = {
  template: `<div><h2>Animais</h2><ul><li>Gato</li><li>Cachorro</li><li>Pássaro</li></ul></div>`
};
const FoodItems = {
  template: `<div><h2>Comidas</h2><ul><li>Pizza</li><li>Hambúrguer</li><li>Sushi</li></ul></div>`
};

export default {
  name: 'ExemploRouter',
  components: {
    'animal-collection': AnimalCollection,
    'food-items': FoodItems
  },
  setup() {
    const activeComp = ref('animal-collection');
    return { activeComp };
  }
};
</script>