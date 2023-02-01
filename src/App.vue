<script setup>
import { ref } from "vue";

let counter = ref(5);
</script>


<template>
  <main>
    <div>
      <h4>The Current count is</h4>
      <h1>{{ counter }}</h1>
      <button @click="counter--">-</button>
      <button @click="counter++">+</button>
    </div>
  </main>
</template>


<style scoped>
main {
  background-color: aliceblue;
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
}

div {
  text-align: center;
}
</style>