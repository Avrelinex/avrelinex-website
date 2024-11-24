<template>
  <div
    class="bg-white section-container flex flex-col justify-center items-center gap-8"
    id="faq"
  >
    <span class="text-[#1C1715] font-medium text-5xl leading-normal text-center">
      Frequently Asked Questions
    </span>

    <div class="flex flex-col gap-4 w-full">
      <FaqItem
        v-for="question in questions"
        :key="question.name"
        :name="question.name"
        :description="question.description"
      />
    </div>
  </div>
</template>

<script setup lang="ts">
import FaqItem from './FaqItem.vue';

const questions = [
  {
    name: "What industries do you specialize in?",
    description: "We focus on EdTech, creating innovative solutions for schools, universities, and corporate training programs.",
  },
  {
    name: "How do you ensure the solutions meet our needs?",
    description: "Our process starts with understanding your goals and challenges. Through open communication and collaboration, we ensure every detail aligns with your vision.",
  },
  {
    name: "What kind of support do you offer after project completion?",
    description: "We provide ongoing support, including maintenance, updates, and training to ensure your solution continues to deliver results.",
  },
  {
    name: "How long does a typical project take?",
    description: "Timelines vary based on project complexity. After the initial consultation, we'll provide a clear roadmap with milestones and delivery dates.",
  },
  {
    name: "Do you offer training for our staff or students?",
    description: "Yes! Training is part of our process to ensure a smooth adoption of the new system by all users.",
  },
  {
    name: "What's the first step to get started?",
    description: "Simply reach out to us! We'll start with a conversation to understand your needs and how we can help you achieve your goals.",
  },
]
</script>
