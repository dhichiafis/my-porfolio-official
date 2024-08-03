<script setup>
import ProjectsViewVue from "./components/ProjectsView.vue";
import {provide} from 'vue'
const projects=[
  {
    'title':'vue js',
    'description':'vue js is a progressive web framework that is based on componet architecture' 
  },
  {
    'title':'fastapi',
    'description':'fastapi is a minimalistic python framework based on pydantic for datavalidation and starlette a python framework for building asyncronouse task'
  },
  {
    'title':'full stack apps',
    'description':'this si teh marriage between two trending frameworks tha i have loved so far for their minimalistic woay of doing thigs'
  }
]
provide('projects',projects)
</script>
<template>
  <div class="px-8">
    <header class='py-6'>

    </header>
    <section class="lg:px-8 sm:px-4">
      <div class="">
        <h1 class="text-center font-bold mx-auto
        text-[45px] lg:leading-[1.2] sm:leading[1.3]">Ochieng Odhiambo</h1>
            
        <div class="grid lg:grid-cols-2 sm:grid-cols-1 mt-6">
          <div class="flex flex-col ">
           <p class="text-left leading-[1.5] text-gray-500 mt-6 text-[22px]">
              i am an ardent software engineer who is interested in providing software solutions 
              geared tower the growth of small to large enterprises
            </p>
            <p class="text-left leading-[1.5] text-gray-500 mt-6 text-[22px]">
              With three years of experience i have worked in a large financial company architecting 
              software solution that has resulted in a massive growth in the revenue line.
              At Mwalimu national i was responsible for building a crm that has maintained over 3000 clients throughout eight teritories
              rustiing in $500000 annual revenue.
            </p>
          </div>
          <div>
            <img src="./assets/2.png" class="lg:w-full sm:min-w-[500px] h-auto">
          </div>
        </div>
      </div>
    </section>
    <section class="lg:px-8 sm:px-4 mt-8">
     <ProjectsViewVue></ProjectsViewVue>
    </section>
  </div>
</template>