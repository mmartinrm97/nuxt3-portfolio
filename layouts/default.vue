<template>
  <div class="container mx-auto">
    <Title>Main Title</Title>
    <nav>
      <NuxtLink to="/">Home</NuxtLink>
      <NuxtLink to="/about">About</NuxtLink>
      <NuxtLink to="/blog">Blog</NuxtLink>
      <NuxtLink to="/blog/my-article">First Article</NuxtLink>
      <NuxtLink to="/todos">Todos</NuxtLink>
    </nav>
    <slot />
  </div>
</template>

<script setup></script>

<style scoped></style>
