<script setup lang="ts">
import { useRoute } from 'vue-router';
import type { Menu } from '@/types/menu';
import Logo from '~/assets/image/logo.svg'

const route = useRoute();
const dropdown = ref<boolean>(false);

const menu = ref<Menu[]>([
  { name: 'home', icon: '', path: '/' },
  { name: 'experiences', icon: '', path: '/experiences' },
  { name: 'technology', icon: '', path: '/technology' },
  { name: 'about', icon: '', path: '/about' },
]);

const activeRouter = computed(()=>{
  return route.path;
})
</script>

<template>
  <div class="flex justify-between items-center w-[80%] mx-auto my-8">
    <h1 class="text-3xl font-bold text-success">
      <NuxtLink to="/">
        <img :src="Logo" alt="logo" />
      </NuxtLink>
    </h1>

    <div class="hidden lg:block">
      <ul class="flex gap-4 capitalize font-semibold">
        <li v-for="tag in menu" :key="tag.name">
          <NuxtLink 
            class="text-lg hover:text-success" 
            :class="{'border-b-4 border-success' : activeRouter === tag.path}"
            :to="tag.path"
          >
            {{ tag.name }}
          </NuxtLink>
        </li>
      </ul>
    </div>

    <div class="flex item-center gap-4">
      <div class="navbar-start block lg:hidden">
        <div class="dropdown">
          <div tabindex="0" role="button" class="btn btn-ghost btn-circle" @click="dropdown = !dropdown">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h7" /> 
            </svg>
          </div>
          <ul
            v-if="dropdown"
            tabindex="0"
            class="menu menu-sm dropdown-content bg-base-100 rounded-box z-1 mt-3 w-52 p-2 z-10 shadow"
          >
            <li v-for="tag in menu" :key="tag.name">
              <NuxtLink 
                @click="dropdown = !dropdown"
                class="hover:text-success" 
                :class="{'underline' : activeRouter === tag.path}"
                :to="tag.path"
              >
                {{ tag.name }}
              </NuxtLink>
            </li>
          </ul>
        </div>
      </div>

      <div class="mt-3 lg:mt-0">
        <label class="grid cursor-pointer place-items-center">
          <input
            type="checkbox"
            value="synthwave"
            class="toggle theme-controller bg-base-content col-span-2 col-start-1 row-start-1" 
          />
          <svg
            class="stroke-base-100 fill-base-100 col-start-1 row-start-1"
            xmlns="http://www.w3.org/2000/svg"
            width="14"
            height="14"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round">
            <circle cx="12" cy="12" r="5" />
            <path
              d="M12 1v2M12 21v2M4.2 4.2l1.4 1.4M18.4 18.4l1.4 1.4M1 12h2M21 12h2M4.2 19.8l1.4-1.4M18.4 5.6l1.4-1.4" />
          </svg>
          <svg
            class="stroke-base-100 fill-base-100 col-start-2 row-start-1"
            xmlns="http://www.w3.org/2000/svg"
            width="14"
            height="14"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round">
            <path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>
          </svg>
      </label>
      </div>
    </div>
  </div>
</template>