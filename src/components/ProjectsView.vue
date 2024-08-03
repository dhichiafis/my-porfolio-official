<script setup>
import {inject} from 'vue'
const projects=inject('projects')
console.log(projects)
</script>
<template>
     <div>
        <h2 class="text-[45px] font-bold text-gray-900 leading-[1.2] text-center ">
          Technical Experience
        </h2>
        <div class="grid lg:grid-cols-3 md:grid-cols-2 mt-4 gap-x-3 gap-y-3">
          <div v-for="i in projects" class=" mt-5 shadow-md lg:px-4 sm:px-8 py-4">
            <h3 class="text-gray-700 leading-[1.2] font-bold
             text-left text-[28px] px-4 mb-3">{{ i.title }}</h3>
            <p class="text-gray-500 text-left px-4 text-[22px]
            leading-[1.5] "> {{ i.description }}</p>
          </div>
        </div>
      </div>
</template>