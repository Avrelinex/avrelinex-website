<template>
  <div
    class="bg-[#FAF7F5] w-full px-32 py-16 flex flex-row justify-center items-center gap-8"
    id="why-us"
  >
    <div class="flex flex-col items-start">
      <span class="text-[#1C1715] font-medium text-5xl leading-normal">
        Why Us?
      </span>
      <span class="text-[#47423F] text-sm">We're here to turn your challenges into opportunities with personalized solutions and ongoing support.</span>
      <OutlineCtaButton class="mt-8"/>
    </div>

    <div class="grid grid-cols-3 gap-8">
      <WhyUsItem
        v-for="benefit in benefits"
        :key="benefit.name"
        :name="benefit.name"
        :icon="benefit.icon"
        :description="benefit.description"
      />
    </div>
  </div>
</template>

<script setup lang="ts">
import WhyUsItem from './WhyUsItem.vue';

const benefits = [
  {
    name: "Clear Communication",
    description: "We believe in maintaining open, transparent communication to understand your needs and keep you informed throughout the entire process.",
    icon: "why-us-communication",
  },
  {
    name: "Fast Feedback Loop",
    description: "We value your input and act quickly to incorporate it, making adjustments to our solutions in real-time and ensuring everything stays on track.",
    icon: "why-us-feedback",
  },
  {
    name: "Ongoing Support",
    description: "Our commitment doesn’t end at launch. We provide continuous support to keep your systems running smoothly and evolving to meet your future needs.",
    icon: "why-us-support",
  },
]
</script>
