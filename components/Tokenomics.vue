<script setup>
import { CoinsIcon, RocketIcon, PercentIcon } from 'lucide-vue-next';

const tokenomics = [
  { title: 'Supply', value: '1,000,000,000', icon: CoinsIcon },
  { title: 'Burned', value: '100%', icon: RocketIcon },
  { title: 'Tax', value: '0%', icon: PercentIcon },
];
</script>

<template>
  <section class="min-h-screen flex items-center justify-center">
    <div class="container mx-auto px-4 py-20">
      <div class="text-center mb-12">
        <h2 class="text-4xl font-bold text-white mb-6">Tokenomics</h2>
        <p class="text-red-200 text-lg">
          Running towards a decentralized future
        </p>
      </div>

      <div class="grid md:grid-cols-3 gap-6">
        <div
          v-for="(item, index) in tokenomics"
          :key="index"
          class="p-6 bg-red-900/40 backdrop-blur-sm border border-red-500/20 rounded-lg"
        >
          <div class="flex flex-col items-center gap-4">
            <component :is="item.icon" class="w-12 h-12 text-red-400" />
            <h3 class="text-xl font-semibold">{{ item.title }}</h3>
            <p class="text-2xl font-bold text-red-300">{{ item.value }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
