<template>
  <section class="relative isolate overflow-hidden" aria-labelledby="hero-title">
    <NuxtImg src="/web-hero-braner-1280x720.jpg" alt="SWC Hero Background"
      class="absolute inset-0 -z-20 h-full w-full object-cover" />

    <div class="absolute inset-0 -z-10 bg-black/35 dark:bg-black/60"></div>
    <div
      class="absolute inset-0 -z-10 bg-linear-to-r from-black/45 via-black/30 to-black/50 dark:from-black/75 dark:via-black/50 dark:to-black/80">
    </div>

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
    <div class="mx-auto grid  grid-cols-1 gap-4 px-4 sm:gap-6 sm:px-6 md:grid-cols-2 md:items-stretch">
      <div class="overflow-hidden rounded-xl border border-(--swc-border) bg-(--swc-surface)">
        <NuxtImg src="/web-800x800.jpg" alt="อุปกรณ์และตู้ไฟสำหรับงานชุบ" class="h-full min-h-64 w-full object-cover" />
      </div>

      <article class="flex flex-col  rounded-xl p-5 ">
        <header>
          <h2 id="product-highlight-title" class="text-xl font-semibold leading-tight sm:text-2xl md:text-3xl">
            ผู้เชี่ยวชาญงานชุบครบวงจร
          </h2>
        </header>

        <p class="mt-4 text-sm leading-7 text-(--swc-text-muted) sm:text-base">
          SWC จำหน่ายอุปกรณ์งานชุบอุตสาหกรรม ตู้ไฟชุบงานมือ 1–มือ 2 น้ำยาชุบนิกเกิล ทองแดง ซิงค์อุปกรณ์โรงงาน
          เครื่องดูดอากาศ เบรคเกอร์ และอะไหล่พร้อมให้คำปรึกษาการเปิดโรงชุบทุกขนาดโดยทีมช่างผู้มีประสบการณ์มากกว่า 20 ปี
        </p>
        <ol class="mt-2 list-decimal list-inside">
          <li class="mx-5 mt-4 flex items-start gap-3 text-sm leading-7 text-(--swc-text-muted) sm:text-base">
            <span class="mt-1 flex h-6 w-6 items-center justify-center text-(--swc-main-color)">
              <Icon name="heroicons:check-circle" class="text-5xl" />
            </span>
            ออกแบบระบบไฟงานชุบ
          </li>
          <li class="mx-5 mt-4 flex items-start gap-3 text-sm leading-7 text-(--swc-text-muted) sm:text-base">
            <span class="mt-1 flex h-6 w-6 items-center justify-center text-(--swc-main-color)">
              <Icon name="heroicons:check-circle" class="text-5xl" />
            </span>
            คำนวณกระแสตามขนาดบ่อ
          </li>
          <li class="mx-5 mt-4 flex items-start gap-3 leading-7 text-(--swc-text-muted) sm:text-base">
            <span class="mt-1 flex h-6 w-6 items-center justify-center text-(--swc-main-color)">
              <Icon name="heroicons:check-circle" class="text-5xl" />
            </span>
            ติดตั้งและเทสระบบหน้างาน
          </li>
          <li class="mx-5 mt-4 flex items-start gap-3 text-sm leading-7 text-(--swc-text-muted) sm:text-base">
            <span class="mt-1 flex h-6 w-6 items-center justify-center text-(--swc-main-color)">
              <Icon name="heroicons:check-circle" class="text-5xl" />
            </span>
            บริการหลังการขาย
          </li>
        </ol>
      </article>
    </div>
  </section>
</template>
<script setup lang="ts">
useSeoMeta({
  title: "ศรีวิชัยโลหะกิจ | จำหน่ายอุปกรณ์การชุบ ตู้ไฟชุบงานมือ 2 น้ำยาชุบ และอุปกรณ์โรงงาน"
});
</script>
