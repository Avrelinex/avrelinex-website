<template>
  <div
    class="flex flex-col px-8 py-5 gap-2 rounded-lg border-2 cursor-pointer transition-all duration-300"
    :class="{
      'border-[#F26A1B]': expanded,
      'border-[#AC9E96]': !expanded,
    }"
    @click="expanded = !expanded"
  >
    <div class="flex flex-row justify-between">
      <span
        class="text-xl font-semibold text-[#1C1715] transition-all"
        :class="{
          'text-[#F26A1B]': expanded,
        }"
      >
        {{ name }}
      </span>
      <nuxt-icon
        name="cross"
        class="h-3 md:h-4 shrink-0 text-[#47423F] transition-all duration-300"
        :class="{
          'text-[#F26A1B] rotate-[-135deg]': expanded,
        }"
      />
    </div>
    <span
      class="text-[#47423F] duration-500"
      :class="{
        'hidden': !expanded,
      }"
    >
      {{ description }}
    </span>
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
})

const expanded = ref(false);
</script>
