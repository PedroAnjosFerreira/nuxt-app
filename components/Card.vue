<script setup lang="ts">
interface CardProps {
  icon: string
  title: string
  members: number
}
const props = defineProps<CardProps>()
</script>
<template>
  <div class="border border-neutral-300 shadow-sm rounded-md overflow-hidden flex">
    <div class="bg-indigo-600 text-white font-bold p-4 flex items-center justify-center w-32">
      <span>{{ props.icon }}</span>
    </div>
    <div class="w-full p-5">
      <h1 class="font-semibold">{{ props.title }}</h1>
      <p class="text-neutral-700">{{ props.members }} membros</p>
    </div>
    <button class="">
      <IconVerticalDots />
    </button>
  </div>
</template>