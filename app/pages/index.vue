<template>
  <section class="relative isolate min-h-screen overflow-hidden" aria-labelledby="hero-title">
    <img src="/web-hero-braner-1280x720.jpg" alt="SWC Hero Background"
      class="absolute inset-0 -z-20 h-full w-full object-cover" />

    <div class="absolute inset-0 -z-10 bg-black/65"></div>
    <div class="absolute inset-0 -z-10 bg-linear-to-r from-black/70 via-black/40 to-black/80"></div>

    <article class="mx-auto flex min-h-screen items-center px-6 md:px-10">
      <header class="flex w-full flex-col items-center gap-6">
        <h1 id="hero-title"
          class=" text-center text-3xl font-light leading-tight tracking-wide text-white sm:text-4xl md:text-5xl">
          เลือกสินค้าที่ตอบโจทย์ ธุรกิจของคุณ
          <br />
          ที่ <span class=" font-bold text-(--swc-red-800)">swc</span>
        </h1>
        <p class="text-center mt-4 text-sm text-white/80 sm:text-base">
          โซลูชันที่เหมาะกับงานติดตั้งและระบบตู้คอนโทรลสำหรับธุรกิจของคุณ
        </p>
      </header>
    </article>
  </section>
</template>
<script setup lang="ts">
useSeoMeta({
  title: "ศรีวิชัยโลหะกิจ | จำหน่ายอุปกรณ์การชุบ ตู้ไฟชุบงานมือ 2 น้ำยาชุบ และอุปกรณ์โรงงาน"
});
</script>