<template>
  <h2>Todo List</h2>
  <!-- <h3>First loop with fetch</h3> -->
  <!-- <ul>
    <li v-for="{ id, title } in todos" :key="id">
      {{ title }}
    </li>
  </ul> -->

  <hr />

  <h3>Second loop with useFetch</h3>
  <ul>
    <li v-for="{ id, title } in todos2" :key="id">
      {{ title }}
    </li>
  </ul>
</template>

<script setup>
// import { ref } from "vue";

const API_URL = "https://jsonplaceholder.typicode.com/todos";
// const todos = ref([]);

// onMounted(async () => {
//   const response = await fetch(API_URL);

//   todos.value = await response.json();
// });

const { data: todos2 } = await useFetch(API_URL);
</script>

<style lang="scss" scoped></style>
