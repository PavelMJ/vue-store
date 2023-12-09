<script setup>
import { ref } from 'vue'

const count = ref(0)
const incriment = () => {
  {
    count.value++
  }
  console.log(count.value)
}
const decriment = () => {
  if (count.value > 0) {
    count.value--
  }
}

const updater = (event) => {
  count.value = Number(event.target.value)
  event.target.value = ''
}
</script>

<template>
  <h3>{{ count }}</h3>
  <input class="countUpdater" type="text" @keyup.enter="updater" />
  <button @click="updater">add</button>

  <div class="btns">
    <button class="btn" @click="incriment">Counter +</button>
    <button class="btn" @click="decriment">Counter -</button>
  </div>
</template>

<style>
/* .btn {
  margin: 5px auto;
  cursor: pointer;
  background: rgb(133, 133, 182);
  color: aliceblue;
  width: 120px;
  height: 40px;
  border: 2px solid #5e5e5e;
  border-radius: 8px;
}
body {
  font-family: sans-serif;
}

.btns {
  display: flex;
  flex-flow: column;
}

.countUpdater {
  text-align: center;
  width: 50px;
  height: 20px;
  font-size: 18px;
} */
</style>
