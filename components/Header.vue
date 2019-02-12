<template>
  <header role="banner">
    <nuxt-link to="/" class="header-icon">Agape Christian Fellowship</nuxt-link>
    <div
      class="navbar-collapse-toggle hamburger"
      :class="{'navbar-active': !mobileHidden}"
      v-on:click="toggleMobileNav"
    >
      <div class="hamburger-line"></div>
      <div class="hamburger-line"></div>
      <div class="hamburger-line"></div>
    </div>
    <nav class="navbar" :class="{'mobile-hidden': mobileHidden}">
      <nuxt-link to="/" class="navbar-link">Home</nuxt-link>
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
