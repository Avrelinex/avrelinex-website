<template>
  <div class="bg-[#FAF7F5] section-container flex flex-row justify-center items-center gap-8 text-center md:text-left">
    <div class="animated w-full flex flex-col jutify-center items-center px-8 py-5 md:px-32 md:py-12 rounded-[2rem] drop-shadow-2xl">
      <div class="flex flex-col jutify-center items-center">
        <span class="text-white font-medium text-[2.5rem] leading-normal">
          Let's Build Something Exceptional Together!
        </span>
        <span class="text-[#FAF7F5]">
          Have questions or ready to start? Reach out today, and let's bring your vision to life!
        </span>
      </div>
      <CtaButton class="mt-8" />
    </div>
  </div>
</template>

<style scoped>
.animated {
	background-size: 200% 200%;
	animation: gradient 8s ease infinite;
  background-image: linear-gradient(135deg, #F26A1B, #5A3D8C, #041E3D);
}


@keyframes gradient {
	0% {
		background-position: 0% 50%;
	}
	50% {
		background-position: 100% 50%;
	}
	100% {
		background-position: 0% 50%;
	}
}
</style>
