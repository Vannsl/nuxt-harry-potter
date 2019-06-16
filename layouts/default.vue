<template>
  <div>
    <the-navbar />
    <div class="flex justify-center h-screen bg-gray-300">
      <div class="container p-8">
        <nuxt />
      </div>
    </div>
  </div>
</template>

<script>
import TheNavbar from '@/components/TheNavbar'

export default {
  components: {
    'the-navbar': TheNavbar
  }
}
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

body {
  background: #eeeeee;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
