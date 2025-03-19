<script setup lang="ts">
import { about } from '~/utils/card'
</script>

<template>
  <section class="my-8">
    <h3 class="text-2xl text-green font-bold mb-4 underline">About</h3>
    
    <div class="grid grid-cols-1 gap-4 lg:grid-cols-4">
      <div v-for="card in about" :key="card.title">  
        <Cards 
          :image="card.image"
          :title="card.title"
          :link="card.link"
        />
      </div>
    </div>
  </section>
</template>