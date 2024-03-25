<template>
    <div>
      <div class="container mx-auto">
        <div class="mx-5 md:mx-20 my-20">
          <div class="pb-5 font-semibold">
            <p class="pb-10 border-b border-gray-200 text-center text-4xl font-mono uppercase">Featured Products</p>
          </div>
  
            <div class="grid grid-cols-2 lg:grid-cols-5 gap-4 lg:gap-8">
            <ProductView
              v-for="product in page_variables.products"
              :key="product.id"
              :product_card_data="product"
            />

          </div>
        </div>
      </div>
    </div>
</template>
  
  <script setup lang="ts">
  import { onMounted, reactive } from 'vue';
  
  interface Product {
    id: number;
    title: string;
    image: string;
    price: number;
    rating: number; 
  }
  
  interface PageVariablesState {
    products: Product[];
  }
  
  let page_variables = reactive<PageVariablesState>({
    products: [],
  });
  
  let get_all_products = async () => {
    try {
      const response = await fetch(`https://fakestoreapi.com/products?limit=10`);
      const data = await response.json();
      page_variables.products = data.map((product: Product) => ({
        ...product,
        rating: Math.floor(Math.random() * 5) + 1, 
      }));
    } catch (error) {
      console.error(error);
    }
  };
  
  onMounted(() => {
    get_all_products();
  });
  </script>