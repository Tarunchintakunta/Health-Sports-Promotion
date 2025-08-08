<template>
    <section class="py-20 bg-white dark:bg-gray-900">
      <div class="container mx-auto px-4">
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
          <!-- Stat item 1 -->
          <div 
            class="bg-gray-50 dark:bg-gray-800 p-8 rounded-xl text-center"
            ref="stat1"
          >
            <div class="text-4xl font-bold text-primary mb-2">
              <span ref="counter1">0</span>+
            </div>
            <div class="text-gray-600 dark:text-gray-400">Community Events</div>
          </div>
          
          <!-- Stat item 2 -->
          <div 
            class="bg-gray-50 dark:bg-gray-800 p-8 rounded-xl text-center"
            ref="stat2"
          >
            <div class="text-4xl font-bold text-secondary mb-2">
              <span ref="counter2">0</span>k
            </div>
            <div class="text-gray-600 dark:text-gray-400">Active Members</div>
          </div>
          
          <!-- Stat item 3 -->
          <div 
            class="bg-gray-50 dark:bg-gray-800 p-8 rounded-xl text-center"
            ref="stat3"
          >
            <div class="text-4xl font-bold text-purple-500 mb-2">
              <span ref="counter3">0</span>+
            </div>
            <div class="text-gray-600 dark:text-gray-400">Sports Facilities</div>
          </div>
          
          <!-- Stat item 4 -->
          <div 
            class="bg-gray-50 dark:bg-gray-800 p-8 rounded-xl text-center"
            ref="stat4"
          >
            <div class="text-4xl font-bold text-red-500 mb-2">
              <span ref="counter4">0</span>%
            </div>
            <div class="text-gray-600 dark:text-gray-400">Health Improvement</div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import { ref, onMounted } from 'vue'
  import gsap from 'gsap'
  import { ScrollTrigger } from 'gsap/ScrollTrigger'
  
  gsap.registerPlugin(ScrollTrigger)
  
  const stat1 = ref(null)
  const stat2 = ref(null)
  const stat3 = ref(null)
  const stat4 = ref(null)
  const counter1 = ref(null)
  const counter2 = ref(null)
  const counter3 = ref(null)
  const counter4 = ref(null)
  
  onMounted(() => {
    // Set up animations for stats
    gsap.from([stat1.value, stat2.value, stat3.value, stat4.value], {
      y: 50,
      opacity: 0,
      stagger: 0.2,
      duration: 0.8,
      ease: "power2.out",
      scrollTrigger: {
        trigger: stat1.value,
        start: "top 80%",
      }
    })
    
    // Animate counters
    gsap.to(counter1.value, {
      innerHTML: 250,
      duration: 2,
      snap: { innerHTML: 1 },
      scrollTrigger: {
        trigger: counter1.value,
        start: "top 80%",
      }
    })
    
    gsap.to(counter2.value, {
      innerHTML: 15,
      duration: 2,
      snap: { innerHTML: 1 },
      scrollTrigger: {
        trigger: counter2.value,
        start: "top 80%",
      }
    })
    
    gsap.to(counter3.value, {
      innerHTML: 120,
      duration: 2,
      snap: { innerHTML: 1 },
      scrollTrigger: {
        trigger: counter3.value,
        start: "top 80%",
      }
    })
    
    gsap.to(counter4.value, {
      innerHTML: 83,
      duration: 2,
      snap: { innerHTML: 1 },
      scrollTrigger: {
        trigger: counter4.value,
        start: "top 80%",
      }
    })
  })
  </script>