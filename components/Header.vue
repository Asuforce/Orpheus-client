<template lang="pug">
  section.hero.is-dark.is-large
    .hero-head
      header.nav
        .container
          .nav-left
            nuxt-link.nav-item.title.is-1.is-spaced(to="/") Orpheus
          .nav-right.nav-menu
            nuxt-link.nav-item.is-active(to="/") Home
            nuxt-link.nav-item(to="/help") Help
            span.nav-item
              nuxt-link.button.is-info.is-inverted(to="/"): span: | Login
</template>
