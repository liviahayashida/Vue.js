<template>
    <Cards>
        <template v-slot:header>
            <h1>SEJAM BEM VINDOS!</h1>
            <p>descrição muito maneira</p>
        </template>
        <main>
            <Cards>
                <!-- conteudo padrao -->
            </Cards>
        </main>
        <template v-slot:footer>
            <p>obrigada pela atenção!</p>
        </template>
    </Cards>
</template>

<script>
import Cards from './Card.vue';
export default {
  components: {
    Cards
  }
}
</script>