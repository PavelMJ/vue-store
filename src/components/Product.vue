<!-- eslint-disable vue/multi-word-component-names -->
<script setup>
defineProps({
  title: String,
  price: Number
})
</script>

<template>
  <div class="product">
    <h2>{{ title }}</h2>
    <h3>Price:{{ `$${price}` }}</h3>
  </div>
</template>

<style>
.product {
  border: 1px solid #5e5e5e;
  padding: 10px;
  margin-bottom: 10px;
}
</style>
