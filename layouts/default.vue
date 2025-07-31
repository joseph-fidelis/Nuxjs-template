<template>
  <div class="min-h-screen flex flex-col bg-[#262626]">
    <!-- Header -->
    <header class=" text-white p-4 ">
      <div class="container mx-auto flex justify-between items-center">
        <NuxtLink to="/" class="text-2xl font-bold">BrickWorks</NuxtLink>
        <nav class="flex space-x-8 items-center">
          <NuxtLink to="/" class="hover:text-black">Home</NuxtLink>
          <NuxtLink to="/features" class="hover:text-black">Features</NuxtLink>
          <NuxtLink to="/pricing" class="hover:text-black">Pricing</NuxtLink>
          <NuxtLink to="/support" class="hover:text-black">Support</NuxtLink>
          <!-- <NuxtLink to="/blog" class="hover:text-blue-300">Blog</NuxtLink> -->
          <NuxtLink to="https://play.google.com/store"
            class="bg-black text-white px-4 py-2 rounded-xl hover:bg-gray-800 transition-colors" target="_blank"
            rel="noopener" >
            Download
          </NuxtLink>
        </nav>
      </div>
    </header>

    <!-- Main Content (slot for page content) -->
    <main class="flex-grow container mx-auto p-4">
      <slot />
    </main>

    <!-- Footer -->
    <footer class=" p-4 mt-auto">
      <div class="container mx-auto text-center">
        <nav class="flex justify-center space-x-16 mb-4 text-gray-400">
          <NuxtLink to="/privacy" class="hover:text-black ">Privacy Policy</NuxtLink>
          <NuxtLink to="/terms" class="hover:text-black">Terms of Service</NuxtLink>
          <NuxtLink to="/blog" class="hover:text-black">Blog</NuxtLink>
          <NuxtLink to="/contact" class="hover:text-black">Contact Us</NuxtLink>
        </nav>
        <p class="text-white">&copy; {{ new Date().getFullYear() }} BrickWorks. All rights reserved.</p>
      </div>
    </footer>
  </div>
</template>

<script lang="ts" setup>
// You can add reactive logic here if needed
</script>

<style scoped> 
/* Add custom styles if needed */
</style>