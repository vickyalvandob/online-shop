<script setup>
import { onMounted } from 'vue'
import { initFlowbite } from 'flowbite'

import Navbar from './Navbar.vue'
import Sidebar from './Sidebar.vue'

// initialize components based on data attribute selectors
onMounted(() => {
    initFlowbite();
})
</script>

<template>
    <div class="antialiased bg-gray-50 dark:bg-gray-900">
  

        <Navbar />
        
        <Sidebar />
        <main class="p-4 md:ml-64 min-h-[100vh] pt-20">
            <slot/>
        </main>
  </div>
</template>