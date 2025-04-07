<template>
  <footer
    class="bg-[#FAF7F5] section-container !py-8 flex flex-col gap-5 md:gap-7"
  >
    <div class="flex flex-row justify-between">
      <div class="flex flex-row md:gap-4 items-center">
        <nuxt-icon name="logo" filled class="h-8" />
        <span
          class="font-bold text-sm text-center md:text-left md:text-base text-black"
          >&copy; 2025 Avrelinex sp. z o. o. All rights reserved.</span
        >
      </div>
      <a href="https://www.linkedin.com/company/avrelinex/" target="_blank">
        <nuxt-icon name="linkedin" filled class="h-6" />
      </a>
    </div>
    <hr />
    <div
      class="flex flex-row text-sm md:text-base font-semibold px-4 justify-center"
    >
      <NuxtLink
        v-for="link in links"
        :key="link.name"
        :to="link.to"
        class="text-gray-800 hover:text-gray-600"
        >{{ link.name }}</NuxtLink
      >
    </div>
  </footer>
</template>

<script setup lang="ts">
const links = [
  {
    name: "Privacy Policy",
    to: "/privacy-policy",
  },
];
</script>
