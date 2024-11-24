<template>
  <div class="flex">
    <button popovertarget="mobile-menu" class="text-[#F26A1B] h-4">
      <nuxt-icon name="menu" />
    </button>
    <div
      popover
      id="mobile-menu"
      class="px-8 py-4 rounded-3xl mt-4 mr-4 shadow-lg border"
    >
      <button popovertarget="mobile-menu" class="text-[#1C1715] absolute right-4 top-4 flex">
        <nuxt-icon
          name="cross"
          class="rotate-45 h-4"
        />
      </button>
      <div class="flex flex-col lg:flex-row gap-5 font-medium justify-center items-center">
        <NuxtLink v-for="link in links" :key="link.to" :to="link.to">
          {{ link.name }}
        </NuxtLink>
        <CtaButton />
      </div>
    </div>
    
  </div>
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
