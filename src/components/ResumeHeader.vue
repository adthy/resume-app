<template>
  <div>
    <div class="flex mx-10 mt-6 mb-3">
      <div class="w-24 h-24 sm:w-16 sm:h-16 mr-2 mt-1">
        <img
          v-if="avatar.selected"
          class="object-cover w-24 h-24 sm:w-16 sm:h-16 rounded-full"
          :src="avatar.url"
          alt=""
        >
      </div>
      <div class="w-2/3 pt-1 pl-2">
        <div class="flex -mb-2 mt-1">
          <span class="text-4xl sm:text-2xl font-bold">
            {{ info.name }}
          </span>
        </div>
        <div class="flex">
          <span class="text-2xl sm:text-base text-gray-600">
            {{ info.position }}
          </span>
        </div>
      </div>
    </div>
    <div class="flex mx-10 mt-8 sm:mt-0 mb-2">
      <span class="text-base text-gray-700">
        {{ info.summary }}
      </span>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    avatar: {
      selected: true,
      url: 'https://images.unsplash.com/photo-1563235453-a57d94b5a552?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80'
    },
    info: {
      name: 'Jonathan Doe',
      position: 'Web Designer',
      summary: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed earum provident amet, impedit excepturi odio nemo minima, cum architecto iure harum tenetur ipsum ipsam id similique, tempora asperiores vel omnis.'
    }
  })
}
</script>

<style>

</style>
