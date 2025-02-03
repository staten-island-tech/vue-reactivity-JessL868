<template>
    <div>
        <h1> {{ produce }}</h1>
    </div>
</template>

<script setup>
defineProps({
    produce: {
        type: String
    }
})
produce  = [
  {name: "Broccoli (per lb)",
    cost: "$2.99"},
  {name: "Cauliflower (per lb)",
    cost: "$2.99"},
  {name: "Apples (per lb)",
    cost: "$1.99"},
  {name: "Oranges (per lb)",
    cost: "$0.99"},
  {name: "Kiwis (per lb)",
    cost: "$0.99"},
  {name: "Bananas (per lb)",
    cost: "$0.65"},
  {name: "Tomatoes (per lb)",
    cost: "$1.99"},
  {name: "Avocados (per lb)",
    cost: "$0.99"},
  {name: "Sweet Potatoes (per lb)",
    cost: "$0.95"},
  {name: "Roma Tomatoes (per lb)",
    cost: "$2.50"},
  {name: "Lettuce (per lb)",
    cost: "$0.99"},
  {name: "Asparagus (per lb)",
    cost: "$1.99"},
  {name: "Blueberries (per lb)",
    cost: "$2.50"},
  {name: "Carrots (per lb)",
    cost: "$0.99"},
  {name: "Strawberries (per lb)",
    cost: "$2.99"},
  {name: "Bell Peppers (per lb)",
    cost: "$2.50"}, 
  {name: "Cucumbers (per lb)",
    cost: "$1.99"},
  {name: "Watermelon (per lb)",
    cost: "$0.40"},
  {name: "Persimmon (per lb)",
    cost: "$0.99"},
  {name: "Honeydew Melon (per lb)",
    cost: "$8.50"}
]
</script>

<style scoped>

</style>