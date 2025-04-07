<template>
  <ContactForm />
  <div
    class="bg-white text-gray-800 px-6 sm:px-12 lg:px-24 2xl:px-[calc((100%-1280px)/2)] pt-32 pb-16"
  >
    <div class="max-w-4xl mx-auto">
      <h1 class="text-4xl font-extrabold mb-8 border-b pb-4">Privacy Policy</h1>

      <div class="mb-8 space-y-2 text-base">
        <p><strong>Effective Date:</strong> April 6, 2025</p>
        <p><strong>Company Name:</strong> Avrelinex</p>
        <p>
          <strong>Address:</strong> Ul. Józefa Piłsudskiego 74/320, 50-020
          Wrocław, Poland
        </p>
        <p>
          <strong>Contact:</strong>
          <a
            href="mailto:avrelinex@gmail.com"
            class="text-blue-600 hover:underline"
          >
            avrelinex@gmail.com
          </a>
          |
          <a
            href="https://avrelinex.com"
            target="_blank"
            class="text-blue-600 hover:underline"
          >
            avrelinex.com
          </a>
        </p>
      </div>

      <section v-for="(section, index) in sections" :key="index" class="mb-10">
        <h2 class="text-2xl font-semibold mb-3 text-gray-900">
          {{ index + 1 }}. {{ section.title }}
        </h2>
        <p class="text-gray-700 leading-relaxed">
          {{ section.content }}
        </p>
      </section>

      <section class="border-t pt-6 mt-12">
        <h2 class="text-2xl font-semibold mb-3 text-gray-900">9. Contact Us</h2>
        <p class="text-gray-700 leading-relaxed">
          If you have questions regarding this Privacy Policy, please contact us
          at
          <a
            href="mailto:avrelinex@gmail.com"
            class="text-blue-600 hover:underline"
          >
            avrelinex@gmail.com </a
          >.
        </p>
      </section>
    </div>
  </div>
</template>

<script setup>
const sections = [
  {
    title: "Introduction",
    content:
      "At Avrelinex, we value your privacy and are committed to protecting your personal data. This Privacy Policy explains how we collect, use, and safeguard information submitted through our website.",
  },
  {
    title: "What Information We Collect",
    content:
      'We only collect personal data that you voluntarily provide via the "Get in Touch" form on our website, including your name, email address, and message.',
  },
  {
    title: "How We Use Your Information",
    content:
      "The information you submit is used solely for responding to your inquiry or for related follow-up communication.",
  },
  {
    title: "Data Storage",
    content:
      "We do not store personal data on our website. Messages are delivered directly to our email and stored securely. We do not delete emails unless requested.",
  },
  {
    title: "Sharing of Data",
    content:
      "We do not share, sell, or disclose your personal information to any third parties.",
  },
  {
    title: "Cookies and Tracking",
    content:
      "Our website does not use cookies or any third-party analytics tools.",
  },
  {
    title: "Your Rights",
    content:
      "If you would like to access, correct, or delete your personal data, please contact us at avrelinex@gmail.com.",
  },
  {
    title: "LinkedIn Button",
    content:
      "Our website includes a button that opens our LinkedIn page. No data is shared with us through this button, but LinkedIn may collect information per their privacy policy.",
  },
];
</script>
