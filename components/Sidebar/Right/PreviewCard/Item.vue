<template>
  <div class="dark:hover:bg-dim-350 cursor-pointer p-3 hover:bg-gray-100" :class="wrapperClasses">
    Item
  </div>
</template>
<script leng="ts" setup>
const { defaulTransition, twitterBorderColor } = useTailwindConfig()
const wrapperClasses = computed(() => `${defaulTransition} ${twitterBorderColor}`)
</script>
