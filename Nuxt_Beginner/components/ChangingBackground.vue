<template>
    <div>
        <div class="relative h-screen">
            <img :class="{ 'opacity-0': currentImage === 1 }" src="~/assets/home-1.jpg" class="rounded-2xl absolute inset-0 w-full h-full object-cover transition-opacity duration-1000" alt="Background Image 1">
            <img :class="{ 'opacity-0': currentImage === 0 }" src="~/assets/home-2.jpg" class="rounded-2xl absolute inset-0 w-full h-full object-cover transition-opacity duration-1000" alt="Background Image 2">
        
        <div class="rounded-2xl absolute inset-0 bg-black opacity-70"></div>
        <div class="absolute inset-0 flex flex-col items-center justify-center text-center">
            <p class="text-xl text-white mb-4 font-thin">Summer Collection</p>
            <h1 class="text-6xl text-yellow-500 font-serif mb-4">INTRODUCING NEW ARRIVALS</h1>
            <p class="text-lg text-white mb-6">Discover our latest collection of trendy items that just arrived!.</p>
            <button class="bg-gray-700 hover:bg-yellow-500 text-white px-6 py-3 rounded-2xl uppercase shadow-md 
            hover:shadow-lg transition duration-300 transform hover:scale-105">View Collection</button>
        </div>
        </div>
    </div>
</template>

<script setup>
    import { ref } from 'vue';
    import { onMounted } from 'vue';
  
    const currentImage = ref(0);
  
    const switchImages = () => {
        currentImage.value = (currentImage.value + 1) % 2;
    };
  
    onMounted(() => {
        setInterval(switchImages, 5000);
    });
    
</script>