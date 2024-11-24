<template>
  <span class="audience text-[#F26A1B]" />
</template>

<style scoped lang="scss">
@import "assets/styles/typed.scss";

.audience {
  @include typed(
    "Universities",
    "Schools",
    "EdTech Startups",
    "Corporate Training",
    "Online Learning",
    (
      delete: 0.05,
    ),
    (
      caret-width: 0.25rem,
    )
  );
}
</style>
