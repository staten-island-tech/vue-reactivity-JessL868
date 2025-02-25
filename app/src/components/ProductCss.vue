<template>
    <div>
      <h2 class="card" >{{ product.name }} <br> {{ product.cost }}</h2>
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
  width: 8.5rem;
  height: 10rem;
  text-align: center;
  display: flex;
  flex-direction: column;
  border: 2px solid black;
  border-radius: 10px;
  object-fit:contain;
  margin: 30px;
  padding-top: 7px;
  box-shadow: 20px 10px 10px gray;
}


</style>