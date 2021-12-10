<script>
export default {
  props: ['text', 'isFirst', 'avatar'],
}
</script>

<template>
  <div 
    v-if="isFirst"
    class="flex hover:bg-gray-800 hover:bg-opacity-30 px-4 py-1"
  >
    <img class="w-10 h-10 rounded-full mr-4" :src="avatar">
    <div>
      <p class="flex items-baseline">
        <span class="text-green-500 mr-2 text-sm">Shadrack Lilan</span>
        <span class="text-xs text-gray-500">14/06/1996</span>
      </p>
      <p class="text-gray-300">{{ text }}</p>
    </div>
  </div>
  <div v-else class="mt-1 hover:bg-gray-800 hover:bg-opacity-30 px-4 py-1">
    <p class="text-gray-300 pl-14">{{ text }}</p>
  </div>
</template>