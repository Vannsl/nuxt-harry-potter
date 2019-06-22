<template>
  <div>
    <the-navbar />
    <div class="flex justify-center h-screen bg-green-600">
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
