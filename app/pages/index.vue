<template>
  <div class="flex flex-col">
    <HeroSection />
    <ServicesSection />
    <WhyUsSection />
    <OurProcessSection />
    <CtaSection />
    <FaqSection />
  </div>
</template>

<script>
import HeroSection from "~/components/HeroSection";
import ServicesSection from "~/components/ServicesSection";
import WhyUsSection from "~/components/WhyUsSection.vue";
import OurProcessSection from "~/components/OurProcessSection.vue";
import CtaSection from "~/components/CtaSection.vue";
import FaqSection from "~/components/FaqSection.vue";

definePageMeta({
  colorMode: "light",
});
</script>
