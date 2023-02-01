<script setup>
import { ref } from "vue";

let counter = ref(0);

const addCount= () =>{
  return counter.value++
}


const redCount = () =>{
  return counter.value = counter.value -1
}
</script>


<template>
  <main>
    <div>
      <h4>The Current count is</h4>
      <h1>{{ counter }}</h1>
      <button @click="redCount()">-</button>
      <button @click="addCount()">+</button>
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