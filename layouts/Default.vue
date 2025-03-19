<template>
  <div class="flex flex-col h-screen">
    <Menu />
      <div class="flex-1 my-4">
        <slot />
      </div>
    <Footer />
  </div>
</template>