<template>
  <div>
    <nav class="navbar">
      <div class="container">
        <div class="navbar-brand">
          <nuxt-link class="navbar-item" to="/">
            <img src="https://www.datocms-assets.com/62239/1643608046-mamawa0.png" alt="Mamawatoto Eco School Logo" />
          </nuxt-link>
          <span class="navbar-burger burger" v-on:click="toggleNavbar">
            <span></span>
            <span></span>
            <span></span>
          </span>
        </div>
        <div :class="['navbar-menu', navbarOpen && 'is-active']">
          <div class="navbar-end">
            <nuxt-link class="navbar-item is-active is-size-5 has-text-weight-semibold" to="/">
              Home
            </nuxt-link>
          </div>
        </div>
      </div>
    </nav>

    <nuxt />

    <footer class="footer">
      <div class="content has-text-centered">
        <p>
          <strong>Mamawatoto Eco School, Machakos Kenya</strong> in partnership with <a href="https://scdhub.org">SCD Hub</a>.  Making use of <a href="https://datocms.com">Dato CMS</a> <a href="https://github.com">Github</a> & <a href="https://netlify.com">Netlify</a></p>
	<p>Code Licensed <a href="https://opensource.org/licenses/GPL-3.0">GPL V3</a>
        </p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navbarOpen: false
    }
  },
  methods: {
    toggleNavbar() {
      this.navbarOpen = !this.navbarOpen
    }
  }
}
</script>

<style>
nav.navbar {
  box-shadow: 0 1px 3px 0 rgba(0, 0, 0, 0.1), 0 1px 2px 0 rgba(0, 0, 0, 0.06) !important;
}
</style>
