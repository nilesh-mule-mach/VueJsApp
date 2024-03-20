<template>
    <div>
    <nav class="bg-gray-800 bg-primary p-4">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex items-center justify-between h-16">
          <!-- Logo -->
          <div class="flex-shrink-0">
            <img src="https://jyn.ai/_nuxt/img/jyn.d706eac.png" class="h-20" alt="Logo">
          </div>
  
          <!-- Navigation links -->
          <div class="hidden md:block">
            <div class="ml-10 flex items-baseline space-x-4">
              <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Home</a>
              <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">About</a>
              <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Services</a>
              <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Contact</a>
            </div>
          </div>
  
          <!-- Hamburger menu for mobile -->
          <div class="-mr-2 flex md:hidden">
            <button @click="isOpen = !isOpen" class="text-gray-300 hover:text-white inline-flex items-center justify-center p-2 rounded-md focus:outline-none focus:bg-gray-700 focus:text-white" :aria-expanded="isOpen ? 'true' : 'false'">
              <span class="sr-only">Open main menu</span>
              <svg class="block h-6 w-6" :class="{'hidden': isOpen, 'block': !isOpen}" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path>
              </svg>
              <svg class="hidden h-6 w-6" :class="{'block': isOpen, 'hidden': !isOpen}" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
              </svg>
            </button>
          </div>
        </div>
      </div>
  
      <!-- Mobile menu -->
      <div class="md:hidden" :class="{'block': isOpen, 'hidden': !isOpen}">
        <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
          <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Home</a>
          <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">About</a>
          <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Services</a>
          <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Contact</a>
        </div>
      </div>
    </nav>
    <div class="bg-cyan-300 relative w-screen h-screen flex justify-center items-center">
    <img src="https://jyn.ai/_nuxt/img/jyn.d706eac.png" class="w-96 h-auto px-4">
</div>

    <footer class="bg-gray-800 bg-primary p-4">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex items-center justify-between">
          <p class="text-white"> © Copyright 2024. All rights reserved.</p>
        </div>
      </div>
    </footer>
</div>
  </template>
   
  <script>
  export default {
    data() {
      return {
        isOpen: false
      }
    }
  }
  </script>
  