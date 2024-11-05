<script setup>
import { ChevronDownIcon } from 'lucide-vue-next';
</script>

<template>
  <section
    class="min-h-screen flex flex-col items-center justify-center text-center p-4"
  >
    <h1
      class="text-5xl md:text-7xl font-bold mb-6 bg-gradient-to-r from-red-500 via-yellow-500 to-purple-500 text-transparent bg-clip-text"
    >
      Found a Runner
    </h1>
    <p class="text-xl md:text-2xl mb-8 text-red-200">
      Journey through the cosmic landscape
    </p>
    <p class="text-xl md:text-2xl mb-8 text-red-200">
      CA: 6uaMSL5XKwk2PESbKvrmmKjhGKkmwboDktSy5tZdpump
    </p>
    <a
      href="https://dexscreener.com/solana/gqqs7cxixqrwu8tbufiznxa1iyunsugunbwrjwnuv2dp"
      target="_blank"
      class="bg-red-600 hover:bg-red-700 text-white px-8 py-4 text-lg rounded-full transition duration-300"
    >
      Join the Run
    </a>
    <div class="absolute bottom-10 animate-bounce">
      <ChevronDownIcon class="w-8 h-8 text-white/60" />
    </div>
  </section>
</template>
