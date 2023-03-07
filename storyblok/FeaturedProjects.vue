<template>
  <div v-editable="blok">
    <!-- Feature projects -->
    <div class="flex flex-col gap-2 lg:gap-2">
      <h3 class="text-base text-head_text md:text-2xl lg:text-4xl">
        {{ blok.title }}
      </h3>
      <p>{{ blok.subtitle }}</p>
      <div
        v-if="blok.projects.length"
        class="mx-auto grid grid-cols-1 gap-7 pt-8 sm:w-5/6 sm:gap-6 lg:w-full lg:grid-cols-2"
      >
        <NuxtLink
          v-for="{ uuid, content } in blok.projects"
          :key="uuid"
          to="/projects"
          class="flex w-full flex-col items-center gap-8 rounded-md border-[1px] border-border_sm bg-item_back p-6 py-6 transition-colors hover:bg-item_hover_back lg:p-6 lg:py-10"
          ><img
            alt="Project 1"
            :src="content.image.filename"
            class="w-full rounded-md object-cover lg:h-48"
          />
          <div class="flex flex-col justify-between gap-4 lg:gap-5">
            <span class="text-lg text-head_text lg:text-xl">{{
              content.name
            }}</span>
            <p class="text-sm md:text-base">{{ content.description }}</p>
          </div></NuxtLink
        >
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  blok: {
    type: Object,
    required: true,
    default: () => ({}),
  },
});
</script>
