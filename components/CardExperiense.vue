<script setup lang="ts">
defineProps<{
  title?: string,
  context?: string[],
  details?: boolean
}>();
</script>

<template>
  <div class="card w-full shadow-sm">
  <div class="card-body">
    <h2 class="text-3xl font-bold">{{title}}</h2>
    <span class="badge badge-warning py-2 px-2 text-base" v-if="details">Atual</span>
    <ul class="mt-2 flex flex-col gap-2" v-for="item in context" :key="item">
      <li>
        <svg 
          xmlns="http://www.w3.org/2000/svg" 
          class="size-4 me-2 inline-block text-success" 
          fill="none" viewBox="0 0 24 24" stroke="currentColor"
        >
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
        <span class="capitalize text-base"> {{item}}</span>
      </li>
    </ul>
  </div>
</div>
</template>