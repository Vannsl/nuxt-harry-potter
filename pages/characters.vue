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
import axios from 'axios'
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
  mounted() {
    axios.get('https://hp-api.herokuapp.com/api/characters')
      .then((response) => {
        this.characters = response.data
      })
  }
}
</script>
