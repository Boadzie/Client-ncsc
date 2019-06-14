<template>
  <div>
    <no-ssr>
      <nav class="navbar is-dark" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
          <nuxt-link
            class="navbar-item"
            to="/"
            style="font-weight:bolder; text-transform:uppercase;letter-spacing:2px;"
          >National Computer Science Challenge</nuxt-link>
          <a
            role="button"
            class="navbar-burger"
            aria-label="menu"
            aria-expanded="false"
            @click="isOpen = !isOpen"
            v-bind:class="{'is-active': isOpen}"
          >
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>
        <div class="navbar-menu" v-bind:class="{'is-active': isOpen}">
          <div class="navbar-end">
            <nuxt-link to="/about" class="navbar-item">Gallery</nuxt-link>
            <nuxt-link to="/" class="navbar-item">Blog</nuxt-link>
            <nuxt-link to="/about" class="navbar-item">About</nuxt-link>
            <nuxt-link to="/contact" class="navbar-item">Contact</nuxt-link>
          </div>
        </div>
      </nav>
    </no-ssr>
  </div>
</template>

<script >
export default {
  data: () => {
    return {
      isOpen: false
    };
  }
};
</script>

<style scoped>
nav {
  font-size: 15px;
}

.navbar-item {
  font-size: 16px;
}
</style>