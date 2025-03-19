<script setup lang="ts">
import { experienseInfo } from '~/utils/card'
</script>

<template>
  <section>
    <h3 class="text-2xl text-green font-bold mb-4 underline">
      Experiences
    </h3>

    <div class="grid grid-cols-1 gap-4 lg:grid-cols-3">
      <div v-for="card in experienseInfo" :key="card.title">
        <CardExperiense 
          :title="card.title"
          :context="card.context"
          :details="card.details"
        />
      </div>
    </div>
  </section>
</template>