<template>
  <div class="flex flex-col gap-5">
    <h3 class="font-theme_bold text-base text-head_text md:text-xl lg:text-2xl">
      Work and education
    </h3>
    <div
      v-for="{ _uid, body } in blok.table.tbody"
      :key="_uid"
      class="flex flex-col gap-2 lg:gap-2"
    >
      <a
        class="flex flex-col flex-nowrap items-start justify-between gap-1 sm:flex-row sm:gap-6"
        href="#"
        ><span class="font-theme_bold text-head_text">{{ body[0].value }}</span
        ><span class="flex-[1_1_auto]"></span
        ><span class="text-sm sm:text-right sm:text-base">{{
          body[1].value
        }}</span
        ><span class="text-sm sm:text-base">{{ body[2].value }}</span></a
      >
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

<style lang="scss" scoped></style>
