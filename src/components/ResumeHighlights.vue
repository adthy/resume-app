<template>
  <div class="mx-10 w-full mb-12 sm:mb-2">
    <div class="flex mt-6 sm:mb-2 w-full">
      <span class="text-red-highlight text-sm tracking-widest uppercase">
        Highlights
      </span>
    </div>
    <div v-for="(item, index) in highlights" :key="index">
      <div class="flex text-gray-600 my-2">
        {{ index + 1 }}. {{ item }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    highlights: [
      'Winner of the Academy Award | Location (url)',
      'Lorem ipsum dolor sit amet consectetur adipisicing elit',
      'Sed earum provident amet, impedit excepturi odio nemo minima'
    ]
  })
}
</script>

<style>

</style>
