<script setup>
import { ref } from "vue";

let count = ref(0);

const addToCount = () => {
  count.value++;
}

const subtractFromCount = () => {
  count.value--;
}
</script>


<template>
  <main>
    <div>
      <h1>VueJS Counter App</h1>
      <h4>The current count is....</h4>
      <h2>{{ count }}</h2>
      <button @click="subtractFromCount">-</button>
      <button @click="addToCount">+</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: aliceblue;
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}
button {
  padding: 10px;
  border-radius: 15px;
  width: 30%;
  background-color: aquamarine;
  margin-top: 20px;
  cursor: pointer;
  font-size: 2rem;
  margin: 8px;
}
</style>