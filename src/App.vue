
<!-- COMPOSITION API -->
<script setup>
import {ref} from "vue"

const count = ref(0);

const addBtn = () => {
  count.value = count.value +1
}

const subtractBtn = () => {
  count.value = count.value -1
}
</script>

<template>
  <div class="header">
   
    <main>
      <h1>this is the current count...</h1>
      <h2>{{ count }}</h2>
      <button @click="subtractBtn">-</button>
      <button @click="addBtn">+</button>
    </main>
  </div>
</template>

<style scoped>
.header {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

main {
  text-align: center;
}
</style>