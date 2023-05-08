<script setup>
const { product } = defineProps(['product'])
</script>

<template>
    <section class="card text-center">
        <NuxtLink :to="`/products/${product.id}`" class="flex flex-col justify-between ">
            <img :src="product.image" alt="product" class="thumb">
            <p class="font-bold text-gray-500 m-4 truncate"> {{ product.title }}</p>
            <p class="btn my-4">View details</p>
        </NuxtLink>
    </section>
</template>

<style scoped>
.thumb {
    max-width: 100px;
    max-height: 120px;
    margin: 0 auto;
    width: 100px;
    height: 120px;
}
</style>