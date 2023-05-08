<script setup>
const { id } = useRoute().params
const url = 'https://fakestoreapi.com/products/' + id
// fetch 
const { data:product } = await useFetch(url)

definePageMeta({
  layout: 'products'
})
if(!product.value){
  throw createError({ctatusCode: 404, statusMessage: 'Product not found', fatal: true})
}
</script>

<template>
  <head>
    <Title>Magazin | {{ product.title }}</Title>
    <Meta name='description' :content="product.description"/>
  </head>
  <div>
    <ProductDitails :product="product"/>
  </div>
</template>