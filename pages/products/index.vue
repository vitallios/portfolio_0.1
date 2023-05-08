
<script setup>
// const {id} = useRoute().params


definePageMeta({
  layout: 'products'
})
// featc 
const { data: products } = await useFetch('https://fakestoreapi.com/products')
useHead({
  title: 'Magazin | Merch',
  meta: [
    {name: 'description', content: 'Nuxt 3 Merch'}
  ]
})
</script>

<template>
  <section class="container">
    <div class="grid grid-cols-4 gap-5">
      <div v-for="p in products" :key="p.title">
        <ProductCars :product="p"/>
      </div>
    </div>
  </section>
</template>