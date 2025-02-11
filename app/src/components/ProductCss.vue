<template>
    <div>
          <h2 class="card">{{ product.name }} <br> {{ product.cost }}</h2>
          <slot></slot>
    </div>
</template>

<script setup>
defineProps ({
  product: Object
})

</script>

<style scoped>
.card {
  width: 8rem;
  height: 10rem;
  text-align: center;
  display: flex;
  flex-direction: column;
  border: 2px solid black;
  object-fit:contain;
  margin: 10px;
  padding-top: 7px;
}
</style>