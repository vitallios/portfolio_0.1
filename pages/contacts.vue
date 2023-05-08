<script setup>
const { data } = await useFetch('/api/ninga')
</script>


<template>
 <section>
  <h2 class="p-5">contacts</h2>
  <p>{{ data }}</p>
 </section>
</template>