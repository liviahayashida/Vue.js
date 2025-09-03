<script setup>
const List = defineList({
    name: String,
    price: Number
})


export default {
  data() {
    return {
      myList: {
        name: '',
        price: '',
      }
    }
  }
}

import { ref, useTemplateRef, onMounted } from 'vue'

const list = ref([
  /* ... */
])

const itemRefs = useTemplateRef('items')

onMounted(() => console.log(itemRefs.value))

const list = defineList({
    name: String,
    price: Number,
})

import {ref} from 'vue'
let inputValue = ref('')

 function mensagem(){
    alert(´Voce comprou ${inputValue}´)
 }

function Increment (){
    this.todos.push({
        id: this.nextTodoId++,
        title: this.newTodoText
      })
      this.newTodoText = ''
    list.value++
    emit('update', list.value)
}

</script>

<template>
<div id="list">
  <input v-model="nextItem"" placeholder="newItem">
  <button @click="addList">Add</button>

  <ul>
    <todo-item
      v-for="todo in todos"
      :key="todo.id"
      :title="todo.title"
      @remove="todos.splice(todos.indexOf(todo), 1)"
    ></todo-item>
  </ul>
</div>


    <div class="card" v-for="name">
        <h3>{{ name }}</h3>
        <span v-for="price">{{ price }} dollars</span>
    </div>


    Vue.component('todo-item', {
  template: '\
    <li>\
      {{ title }}\
      <button v-on:click="$emit(\'remove\')">Remove</button>\
    </li>\
  ',
  props: ['title']
})

new Vue({
  el: '#todo-list-example',
  data: {
    newTodoText: '',
    todos: [
      {
        id: 1,
        title: 'Lavar os pratos',
      },
      {
        id: 2,
        title: 'Tirar o lixo',
      },
      {
        id: 3,
        title: 'Cortar a grama'
      }
    ],
    nextTodoId: 4
  },
  })


<ul>
    <li v-for="item in list" ref="items">
      {{ item }}
    </li>
  </ul>


<div class="list" v-for="value in source">
        <h3>Name: {{ name }}</h3>
        <p>Price: {{ price }} dollars</p>


</div>

 <div>
    <button @click.enter="mensagem">Comprar!</button>
  <input type="text" @keyup.enter="Increment"></input>
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