<template>
    <div>
        <div class="container">
            <h1 class="font">Cart</h1>
            <button class="font" @click="showComponent = false" v-if="showComponent">Hide Products</button>
            <button class="font" @click="showComponent = true" v-if="!showComponent">Show Products</button>
            <h2 class="font" v-if="showComponent" v-for="(item, index) in store.cart" :key="index" :index="index">{{ item.name }} - {{ item.cost }} <button class="font" @click="deleteItem(index)">Remove</button></h2>
        </div>
    </div>
</template>

<script setup>
import { ref } from "vue"
import { store } from '../cart.js'

function deleteItem(index) {
  store.cart.splice(index, 1)
}

let showComponent = ref(true);
</script>

<style scoped>
h1 {
    text-align: center;
}
h2 {
    text-align: center;
    margin-left: 2rem;
    object-fit: contain;
}
.container {
    align-items: center;
    margin-top: 10rem;
    border: 2px solid black;
    border-radius: 10px;
    box-shadow: 20px 10px 10px gray;
}
.font {
    font-family: "DM Sans", serif;
}

</style>
