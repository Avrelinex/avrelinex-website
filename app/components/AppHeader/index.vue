<template>
  <header class="bg-white w-full px-32 py-4 fixed top-0 grid grid-flow-row grid-cols-3 shadow-md items-center z-40">
    <nuxt-icon name="logo-expanded" filled class="h-12 justify-self-start" />
    <Navigation class="justify-self-center" />
    <CtaButton class="justify-self-end" />
  </header>
</template>

<script setup lang="ts">
import Navigation from "./Navigation.vue";
import CtaButton from "./CtaButton.vue";
</script>
