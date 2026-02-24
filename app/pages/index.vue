<template>
  <section class="relative isolate overflow-hidden" aria-labelledby="hero-title">
    <NuxtImg src="/web-hero-braner-1280x720.jpg" alt="SWC Hero Background"
      class="absolute inset-0 -z-20 h-full w-full object-cover" />

    <div class="absolute inset-0 -z-10 bg-black/60"></div>
    <div class="absolute inset-0 -z-10 bg-linear-to-r from-black/75 via-black/50 to-black/80"></div>

    <article class="mx-auto flex min-h-screen items-center px-6 md:px-10">
      <header class="flex w-full flex-col items-center gap-6">
        <h1 id="hero-title"
          class=" text-center text-3xl font-light leading-tight tracking-wide text-white sm:text-4xl md:text-5xl">
          เลือกสินค้าที่ตอบโจทย์ ธุรกิจของคุณ
          <br />
          ที่ <span class=" font-bold text-(--swc-main-color)">swc</span>
        </h1>
        <p class="text-center mt-4 text-sm text-white/80 sm:text-base">
          โซลูชันที่เหมาะกับงานติดตั้งและระบบตู้คอนโทรลสำหรับธุรกิจของคุณ
        </p>
      </header>
    </article>
  </section>

  <section class="bg-(--swc-card) py-8 text-(--swc-text-color) md:py-6" aria-labelledby="product-highlight-title">
    <div class="mx-auto grid max-w-6xl grid-cols-1 gap-4 px-4 sm:gap-6 sm:px-6 md:grid-cols-2 md:items-stretch">
      <div class="overflow-hidden rounded-xl border border-(--swc-border) bg-(--swc-surface)">
        <NuxtImg
          src="/web-800x800.jpg"
          alt="อุปกรณ์และตู้ไฟสำหรับงานชุบ"
          class="h-full min-h-64 w-full object-cover"
        />
      </div>

      <article class="flex flex-col justify-center rounded-xl border border-(--swc-border) bg-(--swc-surface) p-5 sm:p-6 md:p-8">
        <header>
          <h2 id="product-highlight-title" class="text-xl font-semibold leading-tight sm:text-2xl md:text-3xl">
            เลือกสินค้าที่ตอบโจทย์ ธุรกิจของคุณ
            <br />
            ที่ <span class="font-bold text-(--swc-main-color)">swc</span>
          </h2>
        </header>

        <p class="mt-4 text-sm leading-7 text-(--swc-text-muted) sm:text-base">
          จำหน่ายอุปกรณ์การชุบ ตู้ไฟชุบมือ 2 น้ำยาชุบ และอุปกรณ์โรงงานอุตสาหกรรม พร้อมให้คำปรึกษาโดยทีมงานประสบการณ์กว่า 20 ปี
        </p>

        <!-- <div class="mt-6 space-y-3">
          <div class="h-3 w-full rounded bg-(--swc-surface-2)"></div>
          <div class="h-3 w-11/12 rounded bg-(--swc-surface-2)"></div>
          <div class="h-3 w-2/3 rounded bg-(--swc-surface-2)"></div>
        </div> -->
      </article>
    </div>
  </section>
</template>
<script setup lang="ts">
useSeoMeta({
  title: "ศรีวิชัยโลหะกิจ | จำหน่ายอุปกรณ์การชุบ ตู้ไฟชุบงานมือ 2 น้ำยาชุบ และอุปกรณ์โรงงาน"
});
</script>
