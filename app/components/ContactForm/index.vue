<template>
  <div
    popover id="contact-form"
    class="text-[#1C1715] backdrop:backdrop-blur-sm backdrop:bg-[#FAF7F5] backdrop:bg-opacity-30 bg-white border-[#AC9E96] border px-8 py-4 md:px-16 md:py-12 shadow-lg rounded-2xl md:min-w-[35rem]"
  >
    <button class="absolute flex top-4 right-4 md:top-12 md:right-16" popovertarget="contact-form">
      <nuxt-icon name="cross" class="h-3.5 rotate-45" />
    </button>
    <form
      action="https://formsubmit.co/2fed54c3af4bcf37988b7777d5f4adf5"
      method="POST"
      class="flex flex-col"
    >
      <label
        for="name"
        class="font-semibold"
      >
        Name:
      </label>
      <input
        type="text" id="name" name="name" required placeholder="John Doe"
        class="border-b p-1"
      />

      <label
        for="email"
        class="mt-6 font-semibold"
      >
        Email:
      </label>
      <input 
        type="email" id="email" name="email" required placeholder="name@company.com"
        class="border-b p-1"
      />

      <label
        for="message"
        class="mt-6 font-semibold"
      >
        Message:
      </label>
      <textarea
        id="message" name="message" required rows="3"
        class="border rounded-md max-h-60 min-h-12 p-3"
      />

      <button
        type="submit"
        class="bg-[#F26A1B] text-[#FAF7F5] mt-12 rounded-full text-lg px-8 py-2 self-center flex flex-row items-center gap-3"
      >
        <span>Send</span>
        <nuxt-icon name="paper-airplane" class="h-3.5" />
      </button>
    </form>
  </div>
</template>
