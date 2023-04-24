<template>
  <div
    class="m-2 overflow-hidden rounded-2xl border bg-gray-50 dark:bg-dim-700"
    :class="twitterBorderColor"
  >
    <h1
      class="border-b p-3 text-xl font-extrabold text-gray-900 dark:text-white"
      :class="twitterBorderColor"
    >
      {{ props.title }}
    </h1>

    <slot> </slot>

    <div
      class="cursor-pointer p-3 text-sm text-blue-400 hover:bg-gray-100 dark:text-white dark:hover:bg-dim-200"
      :class="defaultTransition"
    >
      Show more
    </div>
  </div>
</template>

<script lang="ts" setup>
const { twitterBorderColor, defaultTransition } = useTailwindConfig()

const props = defineProps({
  title: {
    type: String,
    required: true,
  },
})
</script>
