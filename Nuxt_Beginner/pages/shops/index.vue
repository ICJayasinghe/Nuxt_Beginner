<template>
    <div>
      <div class="grid grid-cols-4 gap-5">
        <div v-for="p in shops">
          <ProductCard :product="p" />
        </div>
      </div>
    </div>
</template>

<script setup>

    const { data: shops } = await useFetch('https://fakestoreapi.com/products')

    useHead({
    title: 'Nuxt Beginner | SHOP',
    meta: [
      { name: 'description', content: 'Nuxt'}
    ]
    })

</script>