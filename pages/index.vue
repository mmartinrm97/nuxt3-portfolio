<template>
  <StoryblokComponent v-if="story" :blok="story.content" />
</template>

<script setup>
const story = await useAsyncStoryblok("home", {
  version: "draft",
  resolve_relations: ["featured-projects.projects"],
});

useHead({
  title: story.value.name,
});
</script>
