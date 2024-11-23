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
</style>