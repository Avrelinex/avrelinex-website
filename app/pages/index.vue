<template>
  <div class="flex flex-col">
    <HeroSection />
    <ServicesSection />
    <WhyUsSection />
    <OurProcessSection />
    <FaqSection />
    <CtaSection />
    <ContactForm />
  </div>
</template>

<script setup lang="ts">
definePageMeta({
  colorMode: "light",
});

useSeoMeta({
  title: "Avrelinex",
});
</script>
