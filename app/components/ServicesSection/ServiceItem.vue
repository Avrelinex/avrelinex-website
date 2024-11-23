<template>
  <div class="bg-[#F0E9E5] flex flex-col px-8 py-5 gap-2.5 rounded-lg drop-shadow-md">
    <span class="text-[#1C1715] text-lg font-semibold">{{ name }}</span>
    <span class="text-[#47423F] text-sm">{{ description }}</span>
  </div>
</template>

<script setup lang="ts">
defineProps({
  name: String,
  description: String,
})
</script>
