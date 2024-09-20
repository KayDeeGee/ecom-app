<template>
    <div>
        <Hero />
    </div>
</template>

<script setup>
const { data, status, error, refresh, clear } = await useFetch('https://api.escuelajs.co/api/v1/products')
</script>

<style scoped></style>