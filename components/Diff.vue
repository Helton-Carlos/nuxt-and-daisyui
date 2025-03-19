<script setup lang="ts">
defineProps<{
  title: string
}>();
</script>

<template>
  <div class="diff aspect-[16/9] my-4 max-h-[90px] md:max-h-[180px]">
    <div class="diff-item-1">
      <div class="bg-success text-success-content grid place-content-center text-2xl font-black lg:text-9xl">
        {{ title }}
      </div>
    </div>
    <div class="diff-item-2">
      <div class="bg-base-200 grid place-content-center text-2xl font-black lg:text-9xl">
        {{title}}
      </div>
    </div>
    <div class="diff-resizer"></div>
  </div>
</template> 