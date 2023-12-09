<script setup>
import ProductVue from './components/Product.vue'
</script>

<template>
  <div class="w-4/5 m-auto bg-white h-screen rounded-lg shadow-xl mt-8">
    <header class="flex justify-between border-b border-slate-300 px-8">
      <div class="flex items-center gap-4">
        <img class="w-10" src="/logo.png" alt="logo" />

        <div class="">
          <div class="tracking-wider -m-0 font-bold text-2xl">Vue Snikers</div>
          <div class="tracking-wide">The Best Snikestore</div>
        </div>
      </div>
      <ul class="flex space-v-4 items-center gap-10">
        <li class="flex items-center gap-3">
          <img src="/cart.svg" alt="Cart" />
          <b>180$</b>
        </li>
        <li class="flex items-center gap-3">
          <img src="/heart.svg" alt="heart" />
          <b>Tabs</b>
        </li>
        <li class="flex items-center gap-3">
          <img src="/profile.svg" alt="Cart" />
          <b>Profile</b>
        </li>
      </ul>
    </header>
  </div>
</template>

<style></style>
