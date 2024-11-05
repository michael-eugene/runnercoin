<script setup>
import { ref } from 'vue'

const pfpPreview = ref('https://hebbkx1anhila5yf.public.blob.vercel-storage.com/photo_2024-11-05_13-49-35-K0XFTFRMUtiEtgwljUiebEBDXgAsUL.jpg')
const runnerName = ref('')

const generatePFP = () => {
  pfpPreview.value = 'https://hebbkx1anhila5yf.public.blob.vercel-storage.com/photo_2024-11-05_12-40-09-e7EKvx1atckiepAScGpNFc1CwqDfoD.mp4'
}

const handleImageError = () => {
  pfpPreview.value = 'https://hebbkx1anhila5yf.public.blob.vercel-storage.com/photo_2024-11-05_13-49-35-K0XFTFRMUtiEtgwljUiebEBDXgAsUL.jpg'
}
</script>

<template>
  <section class="min-h-screen flex items-center justify-center bg-red-900/40 backdrop-blur-sm">
    <div class="container mx-auto px-4 py-20">
      <div class="max-w-md mx-auto text-center">
        <h2 class="text-4xl font-bold text-white mb-6">PFP Generator</h2>
        <p class="text-red-200 text-lg mb-8">Create your unique cosmic runner profile picture</p>
        
        <div class="p-6 bg-black/40 backdrop-blur-sm border border-red-500/20 rounded-lg">
          <div class="space-y-6">
            <div class="relative w-48 h-48 mx-auto">
              <img
                :src="pfpPreview"
                alt="PFP Preview"
                class="object-cover rounded-lg w-full h-full"
                @error="handleImageError"
              />
            </div>
            
            <div class="space-y-4">
              <div>
                <label for="name" class="block text-white mb-2">Runner Name</label>
                <input id="name" v-model="runnerName" class="w-full bg-white/10 border border-red-500/20 text-white rounded-md px-3 py-2" />
              </div>
              
              <button 
                @click="generatePFP"
                class="w-full bg-red-600 hover:bg-red-700 text-white py-2 rounded-md transition duration-300"
              >
                Generate PFP
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>