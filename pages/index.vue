<template>
  <div class="container">
    <div>
      <logo />
      <h1 class="title">
        workshop
      </h1>
      <h2 class="subtitle">
        Workshop: Nuxt.js - VueJS SSR
      </h2>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  head() {
    return {
      meta: [
        {
          name: 'twitter:card', content: 'summary'
        },
        {
          name: 'twitter:site', content: '@Vannsl'
        },
        {
          name: 'twitter:image', content: 'https://www.towa-digital.com/wp-content/uploads/2017/01/team__towa_digitalagentur-1920x1080.jpg'
        },
        {
          name: 'twitter:title', content: 'Nuxt.js Workshop @ TOWA (Bregenz)'
        },
        {
          name: 'twitter:description', content: 'RIGHT NOW we are creating a nuxt.js application which renders aaaall of the amazing Harry Potter characters.'
        }
      ]
    }
  },
  layout: 'light'
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
