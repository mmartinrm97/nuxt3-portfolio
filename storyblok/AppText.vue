<script setup>
import { computed, useAttrs } from "vue";
const props = defineProps({
  blok: {
    type: Object,
    required: true,
    default: () => ({}),
  },
});
const richText = computed(() => renderRichText(props.blok.text));
const defaultCSSClasses =
  "flex flex-col w-full gap-6 mx-auto lg:gap-9 md:w-10/12";
const attrs = useAttrs();
const cssClasses = computed(() => attrs.class || defaultCSSClasses);
</script>

<template>
  <div v-editable="blok">
    <div :class="cssClasses">
      <div v-html="richText"></div>
      <!-- {{ richText }} -->
    </div>
  </div>
</template>

<style scoped>
:deep(p) {
  @apply mb-4 text-sm leading-relaxed last:mb-auto md:text-base lg:leading-8;
}
</style>
