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
  <div v-editable="blok" style="margin-bottom: 40px">
    <h1
      class="font-theme_bold text-xl text-head_text sm:text-3xl md:text-4xl md:leading-normal lg:text-6xl lg:leading-relaxed"
    >
      {{ blok.title }}<span class="text-link_text_hover">.</span>
    </h1>
    <p
      class="sg:leading-8 -mt-2 text-sm leading-relaxed md:text-base lg:text-lg"
    >
      {{ blok.subtitle }}
    </p>
  </div>
</template>
