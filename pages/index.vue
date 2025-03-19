<script setup lang="ts">
import { hardSkill, articles, experienseInfo} from '~/utils/card'
</script>

<template>
  <div>
    <Hero class="my-8" />
    
    <section class="my-8">
      <h3 class="text-2xl text-green font-bold mb-4 underline">Hard Skills</h3>
      
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

    <section class="my-8">
      <Diff title="ARTIGOS" />
      
      <div class="grid grid-cols-1 gap-4 lg:grid-cols-3">
        <div v-for="card in articles" :key="card.title">  
          <Cards 
            :image="card.image"
            :title="card.title"
            :context="card.context"
            :link="card.link"
          />
        </div>
      </div>
    </section>

    <section class="my-8"> 
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

    <section class="grid grid-cols-1 gap-4 lg:grid-cols-2" >
      <MockupAgro />
      <MockupEcommerce />
    </section>
  </div>
</template>