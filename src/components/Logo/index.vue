<template>
  <nuxt-link to="/">
    <img
      class="logo"
      alt="We2geda Logo"
      :src="slogan ? '/images/We2geda-logo-white-tagline.png' : '/images/We2geda-logo-white.png'"
    />
  </nuxt-link>
</template>

<script>
export default {
  props: {
    slogan: {
      type: Boolean,
      default: false
    },
  },
}
</script>
<style>
.logo {
  width: 120px;
}
</style>
