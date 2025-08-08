<template>
    <section class="py-20 bg-white dark:bg-gray-900">
      <div class="container mx-auto px-4">
        <!-- Section header -->
        <div class="text-center mb-16" v-motion :initial="{ opacity: 0, y: 50 }" :visible="{ opacity: 1, y: 0, transition: { duration: 600 } }">
          <h2 class="text-3xl md:text-4xl font-bold mb-4 text-gray-900 dark:text-white">How Our Platform Works</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 max-w-3xl mx-auto">
            Promoting health and well-being through community sport has never been easier.
          </p>
        </div>
        
        <!-- Features grid -->
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- Feature 1 -->
          <div 
            class="bg-gray-50 dark:bg-gray-800 p-8 rounded-xl shadow-sm hover:shadow-md transition-all duration-300"
            v-motion 
            :initial="{ opacity: 0, y: 50 }" 
            :visible="{ opacity: 1, y: 0, transition: { duration: 600, delay: 100 } }"
          >
            <div class="w-14 h-14 bg-blue-100 dark:bg-blue-900 rounded-lg flex items-center justify-center mb-6">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-primary" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
              </svg>
            </div>
            <h3 class="text-xl font-semibold mb-3 text-gray-900 dark:text-white">Find Local Sports</h3>
            <p class="text-gray-600 dark:text-gray-400">
              Discover community sports programs and facilities near you with our interactive map.
            </p>
          </div>
          
          <!-- Feature 2 -->
          <div 
            class="bg-gray-50 dark:bg-gray-800 p-8 rounded-xl shadow-sm hover:shadow-md transition-all duration-300"
            v-motion 
            :initial="{ opacity: 0, y: 50 }" 
            :visible="{ opacity: 1, y: 0, transition: { duration: 600, delay: 200 } }"
          >
            <div class="w-14 h-14 bg-green-100 dark:bg-green-900 rounded-lg flex items-center justify-center mb-6">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-secondary" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
              </svg>
            </div>
            <h3 class="text-xl font-semibold mb-3 text-gray-900 dark:text-white">Book Events</h3>
            <p class="text-gray-600 dark:text-gray-400">
              Register for community sports events and activities with our easy booking system.
            </p>
          </div>
          
          <!-- Feature 3 -->
          <div 
            class="bg-gray-50 dark:bg-gray-800 p-8 rounded-xl shadow-sm hover:shadow-md transition-all duration-300"
            v-motion 
            :initial="{ opacity: 0, y: 50 }" 
            :visible="{ opacity: 1, y: 0, transition: { duration: 600, delay: 300 } }"
          >
            <div class="w-14 h-14 bg-purple-100 dark:bg-purple-900 rounded-lg flex items-center justify-center mb-6">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-purple-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2" />
              </svg>
            </div>
            <h3 class="text-xl font-semibold mb-3 text-gray-900 dark:text-white">Track Progress</h3>
            <p class="text-gray-600 dark:text-gray-400">
              Monitor your health metrics and sports achievements with interactive dashboards.
            </p>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  // @vueuse/motion is automatically available as v-motion directive
  </script>