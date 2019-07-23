<template>
  <div class="w-full flex flex-row border-gray-400 justify-around">
    <div v-for="(item, index) in contact" :key="index" class="ml-0">
      <div class="flex mt-2 w-full">
        <span class="text-sm tracking-widest">
          {{ item.type }}
        </span>
      </div>
      <div>
        <div
          class="text-blue-highlight font-bold flex mb-2"
          v-html="item.value"
        >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    contact: [
      {
        type: 'Website',
        value: `<a href="https://checkme.com/">checkme.com</a>`
      },
      {
        type: 'Email',
        value: `<a href="mailto:textme@mymail.com">textme@mymail.com</a>`
      },
      {
        type: 'Phone',
        value: `<a href="tel:+61 0244286742">+61 02 4428 6742</a>`
      },
    ]
  })
}
</script>
