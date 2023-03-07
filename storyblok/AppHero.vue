<script setup>
defineProps({
  blok: {
    type: Object,
    required: true,
    default: () => ({}),
  },
});
</script>

<template>
  <div v-editable="blok">
    <!-- Hero -->
    <div class="my-10 flex flex-col gap-8">
      <h1
        class="text-xl leading-loose text-head_text sm:text-3xl md:text-4xl xl:text-6xl"
      >
        {{ blok.title }}
        <span class="text-link_text_hover">.</span>
      </h1>
      <p class="text-sm leading-relaxed md:text-2xl">{{ blok.subtitle }}</p>
      <p class="text-sm leading-relaxed md:text-base">{{ blok.text }}</p>
    </div>

    <!-- Contact and social -->
    <div class="flex items-center justify-between" style="margin-top: 24px">
      <div v-if="blok.icons.length" class="flex gap-1">
        <component
          :is="icon.component"
          v-for="icon in blok.icons"
          :key="icon._uid"
          :blok="icon"
          class="mr-1 w-8 rounded-md bg-white p-1 transition-all hover:bg-gray-600"
        />
      </div>
      <div v-if="blok.buttons.length" class="flex gap-2">
        <component
          :is="button.component"
          v-for="button in blok.buttons"
          :key="button._uid"
          :blok="button"
          class="w-fit rounded-md border-[1px] border-link_border bg-btn_back px-2 py-2 text-sm text-btn_text transition-colors hover:bg-border_sm md:px-4"
        />
      </div>
    </div>
  </div>
</template>
