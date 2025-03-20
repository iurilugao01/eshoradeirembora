<script setup>
import confeitti1 from "@/assets/confeitti1.gif";
</script>

<template>
  <div class="container">
    <img :src="confeitti1" alt="" class="confeitti1 mirror" />
    <h1>Hora de ir embora!</h1>
    <img :src="confeitti1" alt="" class="confeitti1" />
  </div>
</template>

<style>
body {
  background-color: #c22525;
  margin: 0;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.container {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 2vh;
  color: #ffe9e9;
  opacity: 0;
  animation: fadeIn 1s ease forwards;
}

@keyframes fadeIn {
  to {
    opacity: 1;
  }
}

h1 {
  font-size: 10vh;
  margin: 0;
  line-height: 1;
}

.confeitti1 {
  width: 20vh;
}

.mirror {
  transform: scaleX(-1);
}
</style>
