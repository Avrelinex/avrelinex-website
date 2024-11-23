<template>
  <div class="bg-[#FAF7F5] grid grid-cols-[2rem_1fr] items-center px-8 py-5 gap-2.5 rounded-lg drop-shadow-lg">
    <nuxt-icon filled :name="icon" class="h-8" />
    <span class="text-[#1C1715] text-3xl font-medium">{{ name }}</span>
    <span class="text-[#47423F] col-start-2">{{ description }}</span>
  </div>
</template>

<script setup lang="ts">
defineProps({
  name: {
    type: String,
    required: true,
  },
  description: {
    type: String,
    required: true,
  },
  icon: {
    type: String,
    required: true,
  },
})
</script>
