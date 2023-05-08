<script setup>
const { product } = defineProps(['product'])
</script>

<template>
    <section class="card">
        <div class="grid grid-cols-2 gap-10">
            <div class="p-7">
                <img :src="product.image" alt="product image" class="mx-auto my-7">
            </div>
            <div class="p-7">
                <h2 class="text-4x1 my-7">{{ product.title }}</h2>
                <p class="text-xl my-7">Pricr - {{ product.price }}</p>
                <h3 class="font-bold border-b-2 mb-4 pb-2">Product descripsion:</h3>
                <p class="mb-7">{{ product.descripsion }}</p>
                <button class="btn flex">
                    <i class="material-icons mr-2">add_shopping_cart</i>
                    <span>Add to card</span>
                </button>
            </div>
        </div>
    </section>
</template>

<style scoped>
img {
    width: 300px;
    height: 300px;
}
</style>