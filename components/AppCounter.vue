<template>
  <h2>{{ total }}</h2>
  <button @click="add">+</button>
  <button @click="substract">-</button>
</template>

<script setup>
import { ref } from "vue";
const total = ref(0);

const add = () => total.value++;

const substract = () => total.value--;
</script>

<style lang="scss" scoped></style>
