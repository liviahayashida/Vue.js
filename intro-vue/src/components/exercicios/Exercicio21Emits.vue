<script setup>
import { ref } from 'vue'

const list = ref([
  { name: 'Produto 1', price: 10 },
  { name: 'Produto 2', price: 20 },
  { name: 'Produto 3', price: 30 }
])

const inputValue = ref('')

function mensagem() {
  alert(`Voce comprou ${inputValue.value}`)
}
</script>

<template>
<div>
  <h2>Lista de Produtos</h2>
  <div class="card" v-for="item in list" :key="item.name">
    <h3>{{ item.name }}</h3>
    <span>{{ item.price }} dollars</span>
  </div>

  <input v-model="inputValue" placeholder="Digite o produto para comprar" />
  <button @click="mensagem">Comprar!</button>
</div>
</template>



<script>
  Vue.component('todo-item', {
    template: '<li>{{ title }} <button @click="$emit(\'remove\')">Remove</button></li>',
    props: ['title']
  });

  new Vue({
    el: '#todo-list-example',
    data: {
      newTodoText: '',
    },
    methods: {
      addList: function () {
        this.todos.push({
          id: this.nextTodoId++,
          title: this.newTodoText
        });
        this.newTodoText = '';
      }
    }
  });
</script>