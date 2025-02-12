<template>
    <div>
        <h1>Cart</h1>
        <h2 v-for="(item, index) in store.cart" :key="index" :index="index">{{ item.name }} - {{ item.cost }}</h2>
    </div>
</template>

<script setup>
import { store } from '../cart.js'
</script>

<style scoped>

</style>
