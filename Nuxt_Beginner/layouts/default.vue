<template>
    <div>
        <header class="shadow-sm bg-gray-800">
            <nav class="grid grid-cols-2 mx-10 py-4">

            <NuxtLink to="/">
                <img src="~/assets/site-logo.png" alt="Logo" class="h-12 justify-start">
            </NuxtLink>
    
            
            <ul class="flex items-center gap-8 justify-end text-sm">
                <li><NuxtLink to="/" class="text-white hover:text-yellow-500 transition duration-300">HOME</NuxtLink></li>
                <li><NuxtLink to="/shops" class="text-white hover:text-yellow-500 transition duration-300">SHOP</NuxtLink></li>
                <li><NuxtLink to="/lookbook" class="text-white hover:text-yellow-500 transition duration-300">LOOKBOOK</NuxtLink></li>
                <li><NuxtLink to="/about" class="text-white hover:text-yellow-500 transition duration-300">ABOUT US</NuxtLink></li>
                <li><NuxtLink to="/contact" class="text-white hover:text-yellow-500 transition duration-300">CONTACT US</NuxtLink></li>
                
                <li>
                <NuxtLink to="/" class="text-yellow-500 hover:text-yellow-300 transition duration-300">
                    <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24">
                    <path fill="currentColor" d="M7 22q-.825 0-1.412-.587T5 20q0-.825.588-1.412T7 18q.825 0 1.413.588T9 20q0 .825-.587 1.413T7 22m10 0q-.825 0-1.412-.587T15 20q0-.825.588-1.412T17 18q.825 0 1.413.588T19 20q0 .825-.587 1.413T17 22M5.2 4h14.75q.575 0 .875.513t.025 1.037l-3.55 6.4q-.275.5-.737.775T15.55 13H8.1L7 15h12v2H7q-1.125 0-1.7-.987t-.05-1.963L6.6 11.6L3 4H1V2h3.25z"/>
                    </svg>
                </NuxtLink>
                </li>
            </ul>
            </nav>
        </header>
        <div class="container mx-auto p-4">
            <slot />
        </div>
    </div>
</template>
  