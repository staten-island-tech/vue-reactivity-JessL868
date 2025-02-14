<template>
    <div>
        <div class="container">
            <h1>Cart</h1>
            <h2 v-for="(item, index) in store.cart" :key="index" :index="index">{{ item.name }} - {{ item.cost }}</h2>
        </div>
    </div>
</template>

<script setup>
import { store } from '../cart.js'
</script>

<style scoped>
h1 {
    text-align: center;
}
h2 {
    text-align: center;
    margin-left: 2rem;
    object-fit: contain;
    height: 50rem;
    width: 50rem;
}
.container {
    margin-top: 10rem;
}
</style>
