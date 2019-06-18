<template>
  <div>
    <h1 class="text-5xl">
      Harry Potter Characters
    </h1>
    <div class="flex flex-wrap justify-around">
      <character
        v-for="character in characters"
        :key="character.name"
        :name="character.name"
        :image="character.image"
        :house="character.house"
        class="w-5/12 mx-1 my-2"
      />
    </div>
  </div>
</template>

<script>
import Character from '@/components/character'

export default {
  name: 'Characters',
  components: {
    character: Character
  },
  data() {
    return {
      characters: []
    }
  },
  async asyncData({ $axios }) {
    const characters = await $axios.$get('https://hp-api.herokuapp.com/api/characters')
    return {
      characters
    }
  }
}
</script>
