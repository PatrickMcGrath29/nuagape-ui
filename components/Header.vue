<template>
  <header role="banner">
    <nuxt-link to="/" class="header-icon">Agape</nuxt-link>
    <div
      class="navbar-collapse-toggle hamburger"
      :class="{'navbar-active': !mobileHidden}"
      @click="toggleMobileNav"
    >
      <div class="hamburger-line" />
      <div class="hamburger-line" />
      <div class="hamburger-line" />
    </div>
    <nav class="navbar" :class="{'mobile-hidden': mobileHidden}">
      <nuxt-link to="/" class="navbar-link">Home</nuxt-link>
      <nuxt-link to="D3" class="navbar-link">D3</nuxt-link>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      mobileHidden: true
    }
  },
  methods: {
    toggleMobileNav() {
      this.mobileHidden = !this.mobileHidden
    }
  }
}
</script>
