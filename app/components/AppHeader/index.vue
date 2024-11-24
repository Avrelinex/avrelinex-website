<template>
  <header class="bg-white section-container !py-4 fixed top-0 flex flex-row justify-between items-center shadow-md z-40">
    <nuxt-icon name="logo-expanded" filled class="h-12" />
    <Navigation class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2" />
    <CtaButton />
  </header>
</template>

<script setup lang="ts">
import Navigation from "./Navigation.vue";
import CtaButton from "./CtaButton.vue";
</script>
