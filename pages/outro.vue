<script setup>
const array = ['Pedro Henrique', 'Caue Henrique', 'Marrgeusd Henrique', 'Vitor Henrique']
const vida = [{
  name: "Pedro", age: 90
},
{
  name: "CAUE", age: 91
}]
</script>
<template>
  <div class="p-10 space-y-5">
    <div class="flex flex-col border-4 rounded-md border-indigo-900 p-3 " v-for="p in vida">
      <span>{{ p.name }}</span>
      <span>{{ p.age }}</span>
    </div>
  </div>
</template>