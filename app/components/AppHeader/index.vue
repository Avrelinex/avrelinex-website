<template>
  <header
    class="bg-white section-container !py-4 fixed top-0 flex flex-row justify-between items-center shadow-md z-40"
  >
    <NuxtLink to="/">
      <nuxt-icon name="logo-expanded" filled class="h-12 cursor-pointer" />
    </NuxtLink>
    <Navigation
      class="max-lg:hidden absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2"
    />
    <MobileNavigation class="lg:hidden" />
    <CtaButton class="max-lg:hidden" />
  </header>
</template>

<script setup lang="ts">
import Navigation from "./Navigation.vue";
import CtaButton from "./CtaButton.vue";
import MobileNavigation from "./MobileNavigation.vue";
</script>
