<template>
  <div class="flex flex-col">
    <HeroSection />
    <ServicesSection />
    <WhyUsSection />
    <OurProcessSection />
    <FaqSection />
    <CtaSection />
  </div>
</template>

<script>
import HeroSection from "~/components/HeroSection";
import ServicesSection from "~/components/ServicesSection";
import WhyUsSection from "~/components/WhyUsSection";
import OurProcessSection from "~/components/OurProcessSection";
import FaqSection from "~/components/FaqSection";
import CtaSection from "~/components/CtaSection";

definePageMeta({
  colorMode: "light",
});
</script>
