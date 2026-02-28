<template>
    <div class="mt-5">
        <article class="mx-auto flex items-center px-6 md:px-10">
            <header class="w-full text-center">
                <h2 id="product-highlight-title" class=" text-xl font-semibold leading-tight sm:text-2xl md:text-3xl">
                    มากกว่า 20 ปีที่เราเป็นส่วนหนึ่งของความสำเร็จในงานชุบของลูกค้า
                </h2>
            </header>
        </article>
        <div class="mx-auto mt-3">
            <div class="overflow-hiddenborder border-(--swc-border) bg-(--swc-surface)">
                <NuxtImg src="/content2-1280x720.jpg" alt="SWC Hero Background"
                    class="inset-0 object-cover w-full h-75" />
            </div>
        </div>
        <div class="mt-5">
            <div class="mx-auto mt-3 grid grid-cols-3 gap-4 px-4 sm:gap-6 sm:px-6 md:grid-cols-3 md:items-stretch">
                <div v-for="value in images" :key="value"
                    class="overflow-hidden rounded-xl border border-(--swc-border) bg-(--swc-surface)">
                    <NuxtImg :src="value" alt="SWC Hero Background" class="inset-0 object-cover w-full h-100" />
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
const images = ref<string[]>();
onMounted(() => {
    images.value = [
        "/content2-400x400-1.jpg",
        "/content2-400x400-2.jpg",
        "/content2-400x400-5.jpg",
    ];
});
</script>
