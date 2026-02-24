<template>
  <footer
    class="border-t text-(--swc-text-light)"
    style="border-color: var(--swc-border); background: linear-gradient(to bottom, var(--swc-red-900), var(--swc-red-800), var(--swc-red-700));"
  >
    <div class="container mx-auto px-4 py-10">
      <div class="grid gap-8 md:grid-cols-3">
        <section class="space-y-3" aria-labelledby="footer-company">
          <h2 id="footer-company" class="text-lg font-semibold tracking-wide">ศรีวิชัยโลหะกิจ (SWC)</h2>
          <p class="text-sm leading-6 text-white/85">
            จำหน่ายอุปกรณ์การชุบ ตู้ไฟชุบงานมือ 2 น้ำยาชุบนิกเกิลและทองแดง พร้อมโซลูชันโลหะชุบ
            และอุปกรณ์โรงงานอุตสาหกรรม โดยทีมช่างและผู้มีประสบการณ์มากกว่า 20 ปี
          </p>
        </section>

        <section class="space-y-3" aria-labelledby="footer-services">
          <h2 id="footer-services" class="text-sm font-semibold uppercase tracking-wider text-white/90">สินค้าและบริการ</h2>
          <ul class="space-y-2 text-sm text-white/85">
            <li>อุปกรณ์การชุบ และอะไหล่ตู้ไฟ</li>
            <li>เครื่องดูดอากาศ เบรคเกอร์ และอุปกรณ์โรงงาน</li>
            <li>ให้คำปรึกษาเปิดโรงชุบขนาดเล็กถึงขนาดใหญ่</li>
          </ul>
        </section>

        <section class="space-y-3" aria-labelledby="footer-contact">
          <h2 id="footer-contact" class="text-sm font-semibold uppercase tracking-wider text-white/90">ติดต่อเรา</h2>
          <div class="space-y-2 text-sm text-white/85">
            <p>Email: swc.service725@gmail.com</p>
            <p>Tel: 061-676-6837</p>
            <a
              href="https://www.facebook.com/swclohakit"
              target="_blank"
              rel="noopener noreferrer"
              class="inline-flex items-center text-white underline decoration-white/40 underline-offset-4 transition hover:decoration-white"
            >
              Facebook: ศรีวิชัยโลหะกิจ
            </a>
          </div>
        </section>
      </div>

      <div class="mt-8 flex flex-wrap items-center justify-between gap-3 border-t border-white/20 pt-4 text-xs text-white/75">
        <p>© {{ currentYear }} ศรีวิชัยโลหะกิจ (SWC). All rights reserved.</p>
        <p>Trusted Service. Quality First.</p>
      </div>
    </div>
  </footer>
</template>

<script setup lang="ts">
const currentYear = useState("current-year", () => new Date().getFullYear());
</script>
