<template>
  <div class="order-first w-7/12">
    <div class="flex mt-6 mb-2">
      <span class="text-red-highlight tracking-widest text-sm uppercase">
        Experience
      </span>
    </div>
    <div v-for="(item, i) in experience" :key="i" class="mb-10">
      <div class="flex my-1">
        <span class="text-md font-bold">
          {{ item.title }}
        </span>
      </div>
      <div class="flex -my-1">
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
  </div>
</template>

<script>
export default {
  data: () => ({
    experience: [
      {
        title: 'Senior Designer @ Company',
        duration: 'Mar 2018 - Feb 2019 | California',
        description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed earum provident amet, impedit excepturi odio nemo minima, cum architecto iure harum tenetur ipsum ipsam id similique, tempora asperiores vel omnis.'
      },
      {
        title: 'Junior Designer @ Company',
        duration: 'Mar 2017 - Mar 2018 | Kansas',
        description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed earum provident amet, impedit excepturi odio nemo minima, cum architecto iure harum tenetur ipsum ipsam id similique, tempora asperiores vel omnis.'
      },
      {
        title: 'Designer @ Company',
        duration: 'Jan 2015 - Feb | Texas',
        description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed earum provident amet, impedit excepturi odio nemo minima, cum architecto iure harum tenetur ipsum ipsam id similique, tempora asperiores vel omnis.'
      },
    ],
  })
}
</script>

<style>

</style>
