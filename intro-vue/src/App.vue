<script setup>
// import UserCard from './components/exercicios/Exemplo10Props.vue'
// const user = {
//     nome: String,
//     email: String,
//     idade: Number,
//     telefone: String,
//     ativo: Boolean
// }
// import EXemplo01 from "./components/exercicios/Exemplo01Interpolacao.vue"
// import EXemplo02 from "./components/exercicios/Exemplo02.vue"
// import EXemplo03 from "./components/exercicios/Exemplo03.vue"
// import {ref} from 'vue'
// import Exemplo02Condicional from "./components/exercicios/Exemplo02Condicional.vue"
//import Exemplo51 from './components/exercicios/Exemplo5-1.vue';
// import Exercicio6Botoes from './components/exercicios/Exercicio6Botoes.vue';
// import Exemplo09 from './components/exercicios/Exemplo09.vue';
// import UserCard from './components/exercicios/Exemplo10Props.vue';
// import ProductCard from './components/exercicios/ProductCard.vue'
// const props = {
//     title: String,
//     price: Number,
//     image: String,
//     inStock: Boolean
// }
// import {ref} from 'vue'
// import Exemplo11Emits from './components/exercicios/Exemplo11Emits.vue';
// const totalCliques = ref(0)
// function atualizarTotal(valor) {
// totalCliques.value = valor
// }
import ExemploSlots from './components/exercicios/atividade01/ExemploSlots.vue';
// import ExemploRouter from './components/exercicios/atividade01/ExemploRouter.vue';
</script>

<template>
<EXemplo01></EXemplo01>
<EXemplo02></EXemplo02>
 <EXemplo03></EXemplo03>
<EXemplo03></EXemplo03>
<Exemplo02Condicional></Exemplo02Condicional>
<Exemplo04></Exemplo04>
<Exercicio6Botoes></Exercicio6Botoes>
<Exemplo09></Exemplo09>
<!-- <UserCard nome="Livia" email="livia.hayshida@aluno.senai.br" idade="17" telefone="1109870987" :ativo="false" ></UserCard> -->
 <!-- <UserCard nome="user.nome" email="livia.hayshida@aluno.senai.br" idade="17" telefone="1109870987" :ativo="false" ></UserCard>
 <ProductCard title="The Adventure" price="20" :image="'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSfqg06wKu_sN1GMm2Uv-62cF3x0jH0cNEH_Q&s'" :inStock="false"></ProductCard> 
 <Exemplo11Emits @update="atualizarTotal"></Exemplo11Emits> -->
 <!-- <p>Total de cliques: {{ totalCliques }}</p> -->
 <Exercicio21Emits></Exercicio21Emits>
 <ExemploSlots></ExemploSlots>
 <ExemploRouter></ExemploRouter>
</template>