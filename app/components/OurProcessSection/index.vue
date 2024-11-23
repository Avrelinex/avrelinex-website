<template>
  <div
    class="bg-white w-full px-32 py-16 flex flex-row gap-8"
    id="our-process"
  >
    <div class="flex flex-col justify-between basis-96">
      <div class="flex flex-col items-start">
        <span class="text-[#1C1715] font-medium text-5xl leading-normal">
          Our process
        </span>
        <span class="text-[#47423F] text-xl">From concept to completion - and <span class="text-[#E81551]">beyond</span>, we're with you every step of the way.</span>
      </div>
      <div class="flex flex-col items-start">
        <span class="text-[#1C1715] font-medium text-[2rem] leading-normal">
          Let's Turn Your Vision into Reality
        </span>
        <span class="text-[#47423F] text-lg">Every project starts with a conversation. Share your vision, and we'll help turn it into reality with precision, care, and support.</span>
        <OutlineCtaButton class="mt-8"/>
      </div>
    </div>

    <div class="flex flex-col gap-8 grow">
      <OurProcessItem
        v-for="step in steps"
        :key="step.name"
        :name="step.name"
        :icon="step.icon"
        :description="step.description"
      />
    </div>
  </div>
</template>

<script setup lang="ts">
import OurProcessItem from './OurProcessItem.vue';

const steps = [
  {
    name: "Discover",
    description: "We start by understanding your goals and challenges, building a solid foundation for a solution that’s perfect for you.",
    icon: "process-discover",
  },
  {
    name: "Design",
    description: "Our team drafts thoughtful designs and prototypes, making sure every detail reflects your vision.",
    icon: "process-design",
  },
  {
    name: "Develop",
    description: "We bring your project to life using cutting-edge technology, ensuring efficiency and quality at every step.",
    icon: "process-develop",
  },
  {
    name: "Deliver",
    description: "We launch your solution with seamless integration and provide training to ensure a smooth transition.",
    icon: "process-deliver",
  },
  {
    name: "Support",
    description: "Post-launch, we stand by you with ongoing maintenance, updates, and support to ensure long-term success.",
    icon: "process-support",
  },
]
</script>
