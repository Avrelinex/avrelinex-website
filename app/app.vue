<template>
  <div>
    <AppHeader />
    <div>
      <NuxtPage />
    </div>
    <AppFooter />
  </div>
</template>

<style>
* {
  font-family: Urbanist;
}

html {
  scroll-behavior: smooth;
}

.nuxt-icon svg {
  margin-bottom: 0;
  width: 100%;
  height: 100%;
}

.section-container {
  @apply w-full py-8 px-8 md:py-16 md:px-16 lg:px-32 2xl:px-[calc((100%-1280px)/2)]
}
</style>