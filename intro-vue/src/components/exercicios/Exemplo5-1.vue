
<template>
  <form @submit.prevent="onSubmit">
    <label for="name">Nome:</label>
    <input type="text" id="name" v-model="name">
        <label for="email">email:</label>
    <input type="text" id="email" v-model="email">
        <label for="idade">idade:</label>
    <input type="number" id="idade" v-model="idade">
        <label for="bio">Biografia:</label>
    <input type="text" id="bio" v-model="bio">
    <button type="submit">Enviar</button>
  </form>
</template>

<script>
export default {
  data() {
    return {
      name: '',
      email: '',
      idade: '',
      bio: ''
    }
  },
  methods: {
    onSubmit() {
      console.log('Nome:', this.name);
      console.log('Email:', this.email);
      console.log('Idade:', this.idade);
      console.log('Biografia:', this.bio);
    }
  }
}
</script>