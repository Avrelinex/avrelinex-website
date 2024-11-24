<template>
  <div
    class="bg-[#FAF7F5] section-container !py-0 h-dvh flex flex-col justify-center items-center gap-8"
  >
    <div class="flex flex-col justify-center items-center">
      <span class="text-[#1C1715] font-medium text-5xl leading-normal">
        Software development for <AnimatedAudience />
      </span>
      <span class="text-xl leading-normal">
        We make sure that your expectations are not only met but <span class="text-[#E81551]">exceeded</span>
      </span>
    </div>
    <LearnMoreButton />
  </div>
</template>

<script setup lang="ts">
import LearnMoreButton from "./LearnMoreButton.vue";
import AnimatedAudience from "./AnimatedAudience.vue";
</script>
