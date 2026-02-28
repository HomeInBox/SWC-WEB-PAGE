<template>
  <header class="border-b bg-(--swc-surface) text-(--swc-text-color)" style="border-color: var(--swc-border);">
    <div class="container mx-auto flex h-16 items-center justify-between px-4">
      <NuxtLink to="/" class="group flex items-center gap-3 rounded-circle">
        <NuxtImg
          src="/logo.svg"
          alt="SWC Logo"
          loading="lazy"
          decoding="async"
          width="64"
          height="64"
          class="h-16 w-16 rounded-circle p-1 transition-transform group-hover:scale-110"
        />
        <span class="hidden text-xs font-semibold uppercase tracking-widest text-(--swc-main-color) sm:block">
          SWC
        </span>
      </NuxtLink>

      <nav class="hidden items-center gap-6 text-sm md:flex">
        <NuxtLink
          to="/"
          class="border-b-2 border-transparent pb-1 transition hover:border-(--swc-main-color) hover:text-(--swc-main-color)"
          exact-active-class="border-(--swc-main-color) text-(--swc-main-color) font-bold"
        >
          รู้จักพวกเรา
        </NuxtLink>
        <NuxtLink
          to="/portfolio"
          class="border-b-2 border-transparent pb-1 transition hover:border-(--swc-main-color) hover:text-(--swc-main-color)"
          exact-active-class="border-(--swc-main-color) text-(--swc-main-color) font-bold"
        >
          ผลงานของเรา
        </NuxtLink>
        <NuxtLink
          to="/products"
          class="border-b-2 border-transparent pb-1 transition hover:border-(--swc-main-color) hover:text-(--swc-main-color)"
          exact-active-class="border-(--swc-main-color) text-(--swc-main-color) font-bold"
        >
          สินค้าของเรา
        </NuxtLink>
        <NuxtLink
          to="/services"
          class="border-b-2 border-transparent pb-1 transition hover:border-(--swc-main-color) hover:text-(--swc-main-color)"
          exact-active-class="border-(--swc-main-color) text-(--swc-main-color) font-bold"
        >
          บริการ
        </NuxtLink>
        <NuxtLink
          to="/contact"
          class="border-b-2 border-transparent pb-1 transition hover:border-(--swc-main-color) hover:text-(--swc-main-color)"
          exact-active-class="border-(--swc-main-color) text-(--swc-main-color) font-bold"
        >
          ติดต่อ
        </NuxtLink>
      </nav>

      <div class="flex items-center gap-3">
        <button
          type="button"
          class="flex items-center gap-2 rounded-full border px-3 py-1 text-xs font-medium text-(--swc-text-color) shadow-sm transition hover:text-(--swc-main-color)"
          style="border-color: var(--swc-border); background: var(--swc-card);"
          aria-label="Toggle dark mode"
          data-theme-toggle
          @click="toggleTheme"
        >
          <span class="h-6 w-6 rounded-full bg-(--swc-gray-300)" :class="{ 'bg-(--swc-main-color)': isDark }"></span>
          <span class="hidden sm:inline">Dark Mode</span>
        </button>

        <button
          type="button"
          class="inline-flex h-9 w-9 items-center justify-center rounded-md border text-(--swc-text-color) md:hidden"
          style="border-color: var(--swc-border); background: var(--swc-card);"
          aria-label="Open menu"
        >
          <span class="block h-0.5 w-4 bg-(--swc-main-color)"></span>
        </button>
      </div>
    </div>

    <div class="border-t bg-(--swc-surface-2) px-4 py-3 md:hidden" style="border-color: var(--swc-border);">
      <div class="flex flex-wrap gap-4 text-sm">
        <NuxtLink to="/" class="text-(--swc-main-color)">รู้จักพวกเรา</NuxtLink>
        <NuxtLink to="/portfolio" class="hover:text-(--swc-main-color)">ผลงานของเรา</NuxtLink>
        <NuxtLink to="/products" class="hover:text-(--swc-main-color)">สินค้าของเรา</NuxtLink>
        <NuxtLink to="/services" class="hover:text-(--swc-main-color)">บริการ</NuxtLink>
        <NuxtLink to="/contact" class="hover:text-(--swc-main-color)">ติดต่อ</NuxtLink>
      </div>
    </div>
  </header>
</template>

<script setup lang="ts">
const { isDark, toggleTheme } = useTheme();
</script>
