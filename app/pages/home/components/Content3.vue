<template>
  <section class="mx-auto mt-10 px-4 sm:px-6 md:px-10">
    <div class="rounded-4xl bg-(--swc-surface) px-4 py-4 sm:px-6 sm:py-6 md:px-8 md:py-8">
      <div
        class="overflow-hidden rounded-3xl border shadow-sm"
        style="border-color: var(--swc-border); background: var(--swc-map-frame);"
      >
        <div class="aspect-video w-full">
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d242.3457299613772!2d100.4085832!3d13.6253903!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x30e2bc8de8d82249%3A0x9381f1050604d898!2z4Lio4Lij4Li14Lin4Li04LiK4Lix4Lii4LmC4Lil4Lir4Liw4LiB4Li04LiIIOC4geC4suC4o-C4iuC4uOC4mg!5e0!3m2!1sen!2sth!4v1772295661818!5m2!1sen!2sth"
            class="h-full w-full transition duration-300"
            :class="{ 'grayscale invert hue-rotate-180 contrast-125 brightness-90': isDark }"
            style="border: 0"
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
const { isDark } = useTheme();
</script>
