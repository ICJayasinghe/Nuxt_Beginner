<template>
    <div class="grid grid-cols-4 grid-rows-2 gap-4 my-4 h-screen px-12">
        <div class="col-span-2 row-span-2 relative">
            <div class="w-full h-full relative rounded-2xl overflow-hidden">
                <img src="~/assets/side-1.jpg" alt="Image 01" class="w-full h-full object-cover rounded-2xl" />
                <div class="absolute inset-0 flex items-center justify-center">
                    <p class="text-white text-4xl font-bold">SUMMER COLLECTION</p>
                </div>
                <div class="absolute inset-0 bg-gradient-to-t from-violet-500 to-transparent opacity-60"></div>
            </div>
        </div>
        <div class="col-span-1 row-span-1 relative">
            <div class="w-full h-full relative rounded-2xl overflow-hidden">
                <img src="~/assets/side-2.jpg" alt="Image 02" class="w-full h-full object-cover rounded-2xl"/>
                <div class="absolute inset-0 flex items-center justify-center">
                    <p class="text-white text-4xl font-bold text-center">MEN'S COLLECTION</p>
                </div>
                <div class="absolute inset-0 bg-gradient-to-t from-yellow-400 to-transparent opacity-60"></div>
            </div>
        </div>
        <div class="col-span-1 row-span-1 relative">
            <div class="w-full h-full relative rounded-2xl overflow-hidden">
                <img src="~/assets/side-3.jpg" alt="Image 03" class="w-full h-full object-cover rounded-2xl"/>
                <div class="absolute inset-0 flex items-center justify-center">
                    <p class="text-white text-4xl font-bold text-center">WOMEN'S COLLECTION</p>
                </div>
                <div class="absolute inset-0 bg-gradient-to-t from-sky-400 to-transparent opacity-60"></div>
            </div>
        </div>
        <div class="col-span-2 row-span-1 relative">
            <div class="w-full h-full relative rounded-2xl overflow-hidden">
                <img src="~/assets/side-4.jpg" alt="Image 04" class="w-full h-full object-cover rounded-2xl"/>
                <div class="absolute inset-0 flex items-center justify-center flex-col">
                    <p class="text-white text-4xl font-bold text-center">FREE SHIPPING</p>
                    <p class="text-white text-lg mt-4">On All Orders Above $299</p>
                    <button class="mt-4 px-5 py-2 bg-white hover:bg-purple-600 text-black hover:text-white text-base rounded-2xl z-10 shadow-md hover:shadow-lg transition duration-300 transform hover:scale-105">View Collection</button>
                </div>
                <div class="absolute inset-0 bg-gradient-to-t from-purple-500 to-transparent opacity-80 rounded-2xl z-0"></div>
            </div>
        </div>
    </div>
</template>


<script setup>

</script>
