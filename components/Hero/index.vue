<template>
    <div class="grid grid-cols-11 gap-4 min-h-[716px] w-full">
        <div class="col-span-1"></div>
        <div class="col-span-9 grid grid-cols-2 gap-1 bg-slate-300">
            <div class="bg-slate-400 h-full w-full relative">
                <NuxtImg :src="data[0].images[0]" alt="" class="object-cover w-full max-h-[716px]" />
                <div class="absolute inset-0 bg-black opacity-30 z-10"></div> <!-- Dark overlay -->
                <h1 class="absolute inset-0 flex items-center justify-center text-9xl font-bold text-white z-20">
                    BEST SELLERS
                </h1>
            </div>
            <div class="grid grid-rows-2 gap-1 bg-slate-400">
                <div class="row-span-1 bg-slate-500">wawa</div>
                <div class="row-span-1 bg-slate-500">
                    <div class="grid grid-cols-12 gap-1 flex-1 h-full">
                        <div class="grid grid-rows-2 gap-1 col-span-6 bg-slate-200">
                            <div class="row-span-1 bg-white">asdasd</div>
                            <div class="row-span-1 bg-white">asdasd</div>
                        </div>
                        <div class="col-span-6 bg-slate-200">asdasd</div>
                    </div>
                </div>
            </div>
        </div>
        <div class="col-span-1 "></div>
    </div>
</template>

<script setup>
const { data, status, error, refresh, clear } = await useFetch('https://api.escuelajs.co/api/v1/products')

</script>

<style scoped></style>