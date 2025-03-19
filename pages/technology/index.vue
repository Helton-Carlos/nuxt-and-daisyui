<script setup lang="ts">
import { hardSkill } from '~/utils/card'
</script>

<template>
  <section class="my-8">
    <h3 class="text-2xl text-green font-bold mb-4 underline">Technology</h3>
    
    <div class="grid grid-cols-1 gap-4 lg:grid-cols-4">
      <div v-for="card in hardSkill" :key="card.title">  
        <Cards 
          :image="card.image"
          :title="card.title"
          :context="card.context"
          :link="card.link"
        />
      </div>
    </div>
  </section>
</template>