<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
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
]
</script>

<template>
  <div class="greetings">
    <h1 class="green">Nature's Basket</h1>
    <div class="container">

    </div>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position:relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
