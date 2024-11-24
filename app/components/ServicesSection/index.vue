<template>
  <div
    class="bg-[#FAF7F5] section-container flex flex-col justify-center items-center gap-8"
    id="services"
  >
    <span class="text-[#1C1715] font-medium text-5xl leading-normal">
      Services
    </span>

    <div class="grid grid-cols-3 gap-8">
      <ServiceItem
        v-for="service in services"
        :key="service.name"
        :name="service.name"
        :description="service.description"
      />
    </div>
  </div>
</template>

<script setup lang="ts">
import ServiceItem from './ServiceItem.vue';

const services = [
  {
    name: "LMS Development",
    description: "Build systems to manage learning and improve student experiences.",
  },
  {
    name: "Admissions Platforms",
    description: "Develop tools to simplify and automate student enrollment processes.",
  },
  {
    name: "Collaboration Tools",
    description: "Develop tools to enhance communication and teamwork in educational environments.",
  },
  {
    name: "Mobile Apps",
    description: "Create apps for learning and simplifying everyday tasks for students and employees.",
  },
  {
    name: "Gamification Solutions",
    description: "Add engaging, interactive features to boost motivation and learning outcomes.",
  },
  {
    name: "Tutorials and Training",
    description: "Provide hands-on training to ensure smooth adoption of new systems.",
  },
]
</script>
