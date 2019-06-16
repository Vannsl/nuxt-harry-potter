<template>
  <div class="flex items-center bg-white">
    <nuxt-link
      to="/"
      class="logo bg-cover block"
    />
    <nuxt-link to="/characters">
      Characters
    </nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'TheNavbar'
}
</script>

<style scoped>
.logo {
  background-image: url('~assets/img/logo-navbar.png');
  height: 80px;
  width: 80px;
}

a:hover {
  color: goldenrod;
}

.nuxt-link-exact-active {
  font-weight: bold;
}
</style>
