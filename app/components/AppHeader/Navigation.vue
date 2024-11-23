<template>
  <nav class="flex flex-row gap-5 font-medium">
    <NuxtLink v-for="link in links" :key="link.to" :to="link.to">
      {{ link.name }}
    </NuxtLink>
  </nav>
</template>

<script setup lang="ts">
const links = [
  {
    name: "Services",
    to: "#services",
  },
  {
    name: "Why Us",
    to: "#why-us",
  },
  {
    name: "Our Process",
    to: "#our-process",
  },
  {
    name: "FAQ",
    to: "#faq",
  },
];

</script>
