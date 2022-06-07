<script setup lang="ts">
interface Card {
  icon: string
  title: string
  members: number
}
const cards: Card[] = [{
  icon: "PD",
  title: "Pedro",
  members: 5,
},
{
  icon: "ඞ",
  title: "Alek",
  members: 1,
},
{
  icon: "DS",
  title: "Doente",
  members: 35,
},
{
  icon: "ADM",
  title: "Lino",
  members: 6,
}, {
  icon: "HG",
  title: "Janio",
  members: 10
}]
</script>
<template>
  <div class="grid grid-cols-4 gap-3 p-5">
    <Card v-for="card in cards" :icon="card.icon" :title="card.title" :members="card.members" />
  </div>
</template>