<script setup>
import { TwitterIcon } from 'lucide-vue-next'
</script>

<template>
  <footer class="bg-black/80 backdrop-blur-sm py-8">
    <div class="container mx-auto px-4">
      <div class="flex flex-col md:flex-row justify-between items-center">
        <div class="text-center md:text-left mb-4 md:mb-0">
          <p class="text-red-200">&copy; 2024 Found a Runner. All rights reserved.</p>
        </div>
        <div class="flex space-x-4">
          <a href="https://x.com/runnercoinsol" class="text-red-200 hover:text-white transition duration-300">
            <TwitterIcon class="w-6 h-6" />
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>