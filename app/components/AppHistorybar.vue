<template>
  <section class="mx-auto mt-10 px-4 sm:px-6 md:px-10">
    <div class="rounded-4xl bg-(--swc-surface) px-6 py-10 text-(--swc-text-color) sm:px-10 md:px-14 md:py-14">
      <header class="text-center">
        <p class="text-sm font-semibold uppercase tracking-[0.35em] text-(--swc-text-muted)">
          History
        </p>
        <h2 class="mt-3 text-2xl font-semibold text-(--swc-text-color) sm:text-3xl md:text-4xl">
          เส้นทางการเติบโตของ SWC
        </h2>
      </header>

      <div class="relative mt-12">
        <div
          class="absolute left-6 right-6 top-4 h-0.75 sm:left-9 sm:right-9"
          style="background: var(--swc-history-track);"
        />

        <div class="grid grid-cols-3 gap-3 sm:gap-6">
          <button
            v-for="item in historyItems"
            :key="item.year"
            type="button"
            class="group relative flex flex-col items-center text-center"
          >
            <span
              class="relative z-10 h-8 w-8 rounded-full border-4 transition-all duration-300 group-hover:scale-110 group-hover:bg-(--swc-main-color)"
              style="border-color: var(--swc-surface); background: var(--swc-history-dot);"
            />
            <div
              class="mt-6 rounded-2xl px-3 py-4 transition-all duration-300 group-hover:-translate-y-1"
              style="background: var(--swc-history-panel);"
            >
              <p class="text-base font-semibold text-(--swc-text-color) transition-colors duration-300 group-hover:text-(--swc-main-color)">
                {{ item.year }}
              </p>
              <p class="mt-2 text-sm leading-6 text-(--swc-text-muted) transition-colors duration-300 group-hover:text-(--swc-text-color)">
                {{ item.description }}
              </p>
            </div>
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
const historyItems = [
  {
    year: '2004',
    description: 'เริ่มต้นธุรกิจด้านอุปกรณ์และระบบงานชุบ พร้อมให้คำปรึกษาหน้างาน',
  },
  {
    year: '2014',
    description: 'ขยายบริการสู่การออกแบบระบบ ติดตั้ง และดูแลโรงงานชุบครบวงจร',
  },
  {
    year: '2024',
    description: 'พัฒนาสินค้าและบริการให้รองรับงานอุตสาหกรรมหลากหลายมากขึ้น',
  },
];
</script>
