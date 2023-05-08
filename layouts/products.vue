<template>
  <div class="container mx-auto p-4">
    <slot />
  </div>


  <footer class="container mx-auto p-4 flex justify-between border-t-2">

    <ul class="flex gap-4">
      <li>
        <NuxtLink to="/contacts">To contacts</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/">To home</NuxtLink>
      </li>
    </ul>

  </footer>
</template>