<template>
  <div class="flex items-center bg-white">
    <nuxt-link
      to="/"
      class="logo bg-cover block"
    />
    <nuxt-link
      to="/characters"
      class="px-1"
    >
      Characters
    </nuxt-link>
    <nuxt-link
      to="/houses/gryffindor"
      class="px-1"
    >
      Gryffindor
    </nuxt-link>
    <nuxt-link
      to="/houses/slytherin"
      class="px-1"
    >
      Slytherin
    </nuxt-link>
    <nuxt-link
      to="/houses/ravenclaw"
      class="px-1"
    >
      Ravenclaw
    </nuxt-link>
    <nuxt-link
      to="/houses/hufflepuff"
      class="px-1"
    >
      Hufflepuff
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
