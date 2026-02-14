<template>
  <footer class="border-t border-red-900/20 bg-gradient-to-b from-red-900 via-red-800 to-red-900 text-white">
    <div class="container mx-auto px-4 py-10">
      <div class="grid gap-6 md:grid-cols-3">
        <div class="space-y-3">
          <div class="text-lg font-semibold tracking-wide">SWC Company</div>
          <p class="text-sm text-white/80">
            เราให้บริการและดูแลด้วยมาตรฐานมืออาชีพ ใส่ใจคุณภาพในทุกขั้นตอน
          </p>
        </div>

        <div class="space-y-3">
          <div class="text-sm font-semibold uppercase tracking-wider text-white/80">ติดต่อเรา</div>
          <div class="space-y-2 text-sm">
            <div class="flex items-center gap-2">
              <span class="h-2 w-2 rounded-full bg-white/70"></span>
              <span>Email: swc.service725@gmail.com</span>
            </div>
            <div class="flex items-center gap-2">
              <span class="h-2 w-2 rounded-full bg-white/70"></span>
              <span>Tel: 061-676-6837</span>
            </div>
          </div>
        </div>

        <div class="space-y-3">
          <div class="text-sm font-semibold uppercase tracking-wider text-white/80">เวลาทำการ</div>
          <div class="text-sm text-white/80">
            จันทร์ - เสาร์: 09:00 - 18:00
          </div>
          <div class="text-sm text-white/80">อาทิตย์: ปิดทำการ</div>
        </div>
      </div>

      <div
        class="mt-8 flex flex-wrap items-center justify-between gap-3 border-t border-white/10 pt-4 text-xs text-white/70">
        <div>© {{ new Date().getFullYear() }} SWC Company. All rights reserved.</div>
        <div class="flex items-center gap-2">
          <span class="h-1.5 w-1.5 rounded-full bg-white/60"></span>
          <span>Trusted Service. Quality First.</span>
        </div>
      </div>
    </div>
  </footer>
</template>
