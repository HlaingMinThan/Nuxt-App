<template>
  <div>
    <Title>Home</Title>
    <h1>home</h1>
    <Counter/>

    <h1>x y mouse coordinates</h1>
    <p>x-{{x}},y{{y}}</p>
  </div>
</template>
<script setup>
  let {x,y}=useMouse()
</script>
