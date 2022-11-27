<script>
import Characters from "./components/Characters.vue";
import "./assets/tailwind.css";

export default {
  components: {
    Characters,
  },
  data() {
    return {
      characters: [],
    }
  },
  mounted() {
    fetch('https://rickandmortyapi.com/api/character')
    .then(res => res.json())
    .then(res => this.characters = res.results)
    .catch(err => console.log(err))
  },
};
</script>

<template>
  <div class="h-screen w-screen">
    <Characters :characters="characters" />
  </div>
</template>
