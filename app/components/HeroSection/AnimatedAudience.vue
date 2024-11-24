<template>
  <span class="audience text-[#F26A1B]" />
</template>

<style scoped lang="scss">
@import "assets/styles/typed.scss";

.audience {
  @include typed("Universities", "Schools", "EdTech Startups", "Corporate Training Programs", "Online Learning Platforms", (delete: .05), (caret-width: 0.25rem));
}
</style>