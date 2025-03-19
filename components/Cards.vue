<script setup lang="ts">
defineProps<{
  image?: string,
  title?: string,
  context?: string,
  link: string
}>();
</script>

<template>
  <div class="card card-compact bg-base-100 w-35 shadow-xl my-4">
    <figure>
      <img
        class="p-4 size-40"
        :src="image"
        :alt="title" 
      />
    </figure>
    <div class="card-body">
      <h2 class="card-title">{{ title }}</h2>
      <p>{{context}}</p>
      <div class="card-actions justify-end">
        <a
          :href="link"
          :alt="title"
          target="_blank"
          class="btn btn-success"
        >Conheça mais</a>
      </div>
    </div>
  </div>
</template>