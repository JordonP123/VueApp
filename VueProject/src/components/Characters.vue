<script>

import Character from './Character.vue'

export default {
  name: "Characters",
  props: {
    characters: Array,
  },
  components: {
   Character
  }
};
</script>

<template>
  <div class="flex flex-wrap justify-evenly">
    <div v-for="character in characters">
    <Character :character="character"/>
    </div>
  </div>
</template>
