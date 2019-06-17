<template>
  <div>
    <h1 class="text-5xl">
      Harry Potter Characters
    </h1>
    <p>
      On this page I will show all Harry Potter characters!
    </p>
  </div>
</template>

<script>
export default {
  name: 'Characters',
  data() {
    return {
      characters: []
    }
  },
  mounted() {
    fetch('https://hp-api.herokuapp.com/api/characters')
      .then((response) => {
        response.json().then((characters) => {
          this.characters = characters
        })
      })
  }
}
</script>
