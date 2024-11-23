<template>
  <div class="bg-white flex flex-col items-center px-8 py-5 gap-2.5 rounded-lg drop-shadow-lg">
    <div class="bg-[#FAF7F5] w-16 h-16 flex justify-center items-center rounded-full drop-shadow-md">
      <nuxt-icon filled :name="icon" class="h-8" />
    </div>
    <span class="text-[#1C1715] text-lg font-semibold">{{ name }}</span>
    <span class="text-[#47423F] text-sm text-center">{{ description }}</span>
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
