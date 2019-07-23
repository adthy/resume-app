<template>
  <div>
    <div class="flex mt-6 sm:mb-2">
      <span class="text-red-highlight text-sm tracking-widest uppercase">
        Education
      </span>
    </div>
    <div v-for="(item, i) in education" :key="i" class="mb-4 sm:mb-6">
      <div class="flex my-1">
        <span class="text-md font-bold">
          {{ item.title }}
        </span>
      </div>
      <div class="flex">
        <span class="text-sm text-gray-500 font-medium">
          {{ item.duration }}
        </span>
      </div>
      <div class="flex my-1">
        <span class="text-sm font-normal">
          {{ item.description }}
        </span>
      </div>
    </div>
    <div class="flex mt-6 sm:mb-2">
      <span class="text-red-highlight text-sm tracking-widest uppercase">
        Core Skills
      </span>
    </div>
    <div
      class="text-sm text-gray-700 sm:hidden"
      v-text="skills.join(', ')"
    >
    </div>
    <div class="hidden sm:inline" v-for="(item, i) in skills" :key="i">
      <div class="my-1">
        <span class="text-sm text-gray-700">
          {{ item }}
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    education: [
      {
        title: 'ETH Zurich',
        duration: '2013-2015',
        description: 'Master of Interaction Design and Cinematography'
      },
      {
        title: 'UC Berkeley',
        duration: '2009-2013',
        description: 'Bachelor of Design'
      }
    ],
    skills: [
      'Animation Design',
      'Front End Design',
      'JavaScript Programming',
      'Back End Software',
      'Node.js'
    ],
  })
}
</script>

<style>

</style>
