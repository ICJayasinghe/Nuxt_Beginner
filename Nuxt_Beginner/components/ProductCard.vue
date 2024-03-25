<template>
  <div class="card text-center">
    <img :src="`${product.image}`" class="h-32 w-32 m-auto" />
    <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
    <NuxtLink :to="`/shops/${product.id}`">
      <p class="btn my-4">View Details</p>
    </NuxtLink>
  </div>
</template>

<script setup>
  const { product } = defineProps(['product'])
</script>
