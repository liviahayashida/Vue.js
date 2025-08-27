<!-- Exercicio de Props 27/08/25 -->

<script setup>
const props = defineProps({
    title: String,
    price: Number,
    image: String,
    inStock: Boolean
})

</script>

<template>
    <div class="card" v-if="title">
        <h3>{{ title }}</h3>
        <br><span v-if="price">Price: {{ price }} dollars</span></br>
        <br><img v-if="image" :src="image"</img></br>
        <div class="inStock ? 'yes' : 'no'"> Does it has an stock? {{ inStock ? "yes" : "no" }}</div>
    </div>
</template>

<style scoped>
.card{
    border: 5px solid rgb(93, 99, 204);
    border-radius: 10px;
    padding: 1rem;
    margin: 1rem;
    background-color: rgb(170, 226, 245);

}

.yes{
    color: #00e100
}

.no{
    color: red
}
</style>