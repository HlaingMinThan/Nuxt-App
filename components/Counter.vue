<template>
  <h1>Counter</h1>

  <h3>count - {{ count }}</h3>
  <h3>plus one count - {{ plusOne }}</h3>

  <button @click="increment">Increment</button>
  <button @click="decrement">Decrement</button>
</template>

<script setup>

let count = ref(0);
let plusOne=computed(()=>count.value+1);
function increment(){
    count.value++;
}
function decrement(){
    count.value--;
}
</script>