<script>

export default {
  name: "Character",
  props: {
    character: Object,
  },
};

</script>

<template>
  <div class="w-18 p-5 m-2 bg-indigo-300">
    <h2 class="text-2xl text-center font-mono text-red-600">{{ character.name }}</h2>
    <img class="m-auto max-w-[250px]" :src="character.image">
    <ul class="p-3">
    <li class="pb-3 text-2xl font-mono text-red-600">Name: {{ character.name }}</li>
    <li class="pb-3 text-2xl font-mono text-red-600">Species: {{ character.species }}</li>
    <li class="pb-3 text-2xl font-mono text-red-600">Status: {{ character.status }}</li>
    <li class="pb-3 text-2xl font-mono text-red-600">Gender: {{ character.gender }}</li>

    </ul>
  </div>
</template>
