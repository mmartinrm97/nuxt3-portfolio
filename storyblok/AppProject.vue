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
    <div class="flex flex-col items-center gap-8">
      <img
        :alt="blok.image.alt"
        :src="blok.image.filename"
        class="w-full rounded-lg"
      />
      <div class="items-left flex flex-col gap-6 md:w-5/6">
        <span class="font-theme_bold text-2xl text-head_text">{{
          blok.name
        }}</span>
        <p class="text-sm lg:text-lg">{{ blok.description }}</p>
        <template v-if="blok.buttons.length">
          <component
            :is="button.component"
            v-for="button in blok.buttons"
            :key="button._uid"
            :blok="button"
            class="font-theme_bold slg:text-base slg:px-6 slg:py-3 w-fit rounded-md border-[1px] border-link_border bg-btn_back px-2 py-2 text-sm text-btn_text transition-colors hover:bg-border_sm md:px-4"
          />
        </template>
      </div>
    </div>
  </div>
</template>
