<template>
    <div>
    <nav class="bg-gray-800 bg-primary p-4">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex items-center justify-between h-16">
          <div class="flex-shrink-0">
            <img src="https://jyn.ai/_nuxt/img/jyn.d706eac.png" class="h-20" alt="Logo">
          </div>
  
          <div class="hidden md:block">
            <div class="ml-10 flex items-baseline space-x-4">
              <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Home</a>
              <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">About</a>
              <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Contact</a>
            </div>
          </div>
  
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

<div class="bg-gray-800 text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">
	<footer class="max-w-screen-xl mx-auto px-4 py-10 sm:px-6 lg:px-8 footer">
		<div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-4 gap-6 mb-10">
			<div>
				<a href="/"><img class="h-20" src="https://jyn.ai/_nuxt/img/jyn.d706eac.png" alt="jynAi"></a>
				<p class="mt-3 text-xs sm:text-sm">© 2024 jyn.ai</p>
			</div>
			<div>
				<div class="grid text-sm">
					<p class="my-1"><a href="/">Home</a></p>
					<p class="my-1"><a href="/join-waitlist/">Join Waitlist</a></p>
					<p class="my-1"><a href="/login/">Login</a></p>
				</div>
			</div>
			<div>
				<div class="grid text-sm">
					<h4 class="uppercase text-base font-normal mb-0 mt-0">World Head Office</h4>
					<div class="mt-0 grid text-sm">
						<p class="leading-6 mt-0">4275 Executive Sq
							<br> La Jolla, CA 92037
							<br> United States</p>
					</div>
				</div>
			</div>
			<div>
				<h4 class="uppercase text-base font-normal">AMERICAS</h4>
				<div class="mt-0 text-sm">
					<p class="mt-0">+1.619.900.9595
						<br> +1.844.900.9595 Toll Free</p>
				</div>
				<h4 class="uppercase text-base font-normal">EMEA</h4>
				<div class="mt-0 text-sm">
					<p class="mt-0">+44.11.3310.0146</p>
				</div>
				<h4 class="mt-7 uppercase text-base font-normal mb-0">APAC</h4>
				<div class="mt-0 text-sm">
					<p class="mt-0">+91.20.4860.9600</p>
				</div>
			</div>
		</div>
		
	</footer>
</div>
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
  