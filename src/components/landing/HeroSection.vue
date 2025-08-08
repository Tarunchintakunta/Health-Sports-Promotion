<template>
    <section class="relative overflow-hidden py-20 md:py-32">
      <!-- Background gradient -->
      <div class="absolute inset-0 bg-gradient-to-br from-blue-50 to-blue-100 dark:from-gray-900 dark:to-gray-800"></div>
      
      <!-- Content -->
      <div class="container mx-auto px-4 relative z-10">
        <div class="flex flex-col md:flex-row items-center">
          <!-- Text content -->
          <div class="md:w-1/2 mb-12 md:mb-0" v-motion :initial="{ opacity: 0, y: 100 }" :visible="{ opacity: 1, y: 0, transition: { duration: 800 } }">
            <h1 class="text-4xl md:text-6xl font-bold mb-6 leading-tight text-gray-900 dark:text-white">
              Promoting Health Through 
              <span class="text-primary-dark dark:text-primary-light">Community Sport</span>
            </h1>
            <p class="text-xl text-gray-700 dark:text-gray-300 mb-8">
              Empowering underrepresented communities through accessible sports programs, education, and resources.
            </p>
            <div class="flex flex-wrap gap-4">
              <button class="px-8 py-4 bg-primary hover:bg-primary-dark text-white font-medium rounded-lg transition duration-300 transform hover:scale-105">
                Get Started
              </button>
              <button class="px-8 py-4 border-2 border-primary text-primary dark:text-white hover:bg-primary/10 font-medium rounded-lg transition duration-300">
                Learn More
              </button>
            </div>
          </div>
          
          <!-- Hero image -->
          <div class="md:w-1/2" v-motion :initial="{ opacity: 0, x: 100 }" :visible="{ opacity: 1, x: 0, transition: { duration: 800, delay: 200 } }">
            <div class="bg-gradient-to-br from-blue-400 to-purple-500 rounded-xl shadow-2xl w-full h-80 flex items-center justify-center">
              <div class="text-white text-center">
                <svg class="w-24 h-24 mx-auto mb-4" fill="currentColor" viewBox="0 0 24 24">
                  <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"/>
                </svg>
                <p class="text-xl font-semibold">Community Sports</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      
      <!-- Floating elements -->
      <div class="absolute -top-20 -right-20 w-80 h-80 bg-blue-400 dark:bg-blue-600 rounded-full opacity-10 blur-3xl"></div>
      <div class="absolute -bottom-40 -left-40 w-80 h-80 bg-green-400 dark:bg-green-600 rounded-full opacity-10 blur-3xl"></div>
    </section>
  </template>
  
  <script setup>
  // @vueuse/motion is automatically available as v-motion directive
  </script>