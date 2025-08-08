<template>
    <section class="py-20 bg-gray-50 dark:bg-gray-800">
      <div class="container mx-auto px-4">
        <div class="flex flex-col lg:flex-row items-center gap-12">
          <!-- Image section -->
          <div class="lg:w-1/2 relative" v-motion :initial="{ opacity: 0, x: -100 }" :visible="{ opacity: 1, x: 0, transition: { duration: 800 } }">
            <div class="rounded-2xl overflow-hidden shadow-xl">
              <div class="bg-gradient-to-br from-green-400 to-blue-500 w-full h-80 flex items-center justify-center">
                <div class="text-white text-center">
                  <svg class="w-24 h-24 mx-auto mb-4" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M16 4c0-1.11.89-2 2-2s2 .89 2 2-.89 2-2 2-2-.89-2-2zm4 18v-6h2.5l-2.54-7.63A1.5 1.5 0 0 0 18.54 8H17c-.8 0-1.54.37-2.01 1l-1.7 2.55c-.19.28-.3.61-.3.95V18h-2v-6h-2v6H9V9c0-.34-.11-.67-.3-.95L7.01 9A2.01 2.01 0 0 0 5 8H3.46c-.8 0-1.54.37-2.01 1L1.5 16.5H4v6h2v-6h2v6h2v-6h2v6h2v-6h2v6h2z"/>
                  </svg>
                  <p class="text-xl font-semibold">Community</p>
                </div>
              </div>
            </div>
            <!-- Floating stats card -->
            <div class="absolute -bottom-6 -right-6 bg-white dark:bg-gray-900 p-6 rounded-xl shadow-lg w-48 border border-gray-100 dark:border-gray-700"
                 v-motion :initial="{ opacity: 0, scale: 0.8 }" :visible="{ opacity: 1, scale: 1, transition: { delay: 400, duration: 500 } }">
              <div class="text-4xl font-bold text-primary mb-2">2,500+</div>
              <div class="text-gray-600 dark:text-gray-400 text-sm">Community members joined last month</div>
            </div>
          </div>
          
          <!-- Content section -->
          <div class="lg:w-1/2" v-motion :initial="{ opacity: 0, x: 100 }" :visible="{ opacity: 1, x: 0, transition: { duration: 800 } }">
            <h2 class="text-3xl md:text-4xl font-bold mb-6 text-gray-900 dark:text-white">Join Our Thriving Community</h2>
            <p class="text-xl text-gray-600 dark:text-gray-400 mb-8">
              Connect with like-minded individuals who are passionate about health and community sports. Share experiences, get inspired, and grow together.
            </p>
            
            <!-- Community features -->
            <ul class="space-y-4 mb-8">
              <li class="flex items-start">
                <div class="flex-shrink-0 w-6 h-6 rounded-full bg-green-100 dark:bg-green-900 flex items-center justify-center mr-3 mt-1">
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 text-green-500" viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd" />
                  </svg>
                </div>
                <span class="text-gray-700 dark:text-gray-300">Join community groups based on your interests</span>
              </li>
              <li class="flex items-start">
                <div class="flex-shrink-0 w-6 h-6 rounded-full bg-green-100 dark:bg-green-900 flex items-center justify-center mr-3 mt-1">
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 text-green-500" viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd" />
                  </svg>
                </div>
                <span class="text-gray-700 dark:text-gray-300">Participate in community-led events and challenges</span>
              </li>
              <li class="flex items-start">
                <div class="flex-shrink-0 w-6 h-6 rounded-full bg-green-100 dark:bg-green-900 flex items-center justify-center mr-3 mt-1">
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 text-green-500" viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd" />
                  </svg>
                </div>
                <span class="text-gray-700 dark:text-gray-300">Access exclusive health and sports resources</span>
              </li>
            </ul>
            
            <button class="px-8 py-4 bg-primary hover:bg-primary-dark text-white font-medium rounded-lg transition duration-300 transform hover:scale-105">
              Join Community
            </button>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  // @vueuse/motion is automatically available as v-motion directive
  </script>