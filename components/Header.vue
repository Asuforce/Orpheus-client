<template>
  <section class="hero is-dark is-large">
    <div class="hero-head">
      <header class="nav">
        <div class="container">
          <div class="nav-left">
            <nuxt-link to="/" class="nav-item title is-1 is-spaced">
              Orpheus
            </nuxt-link>
          </div>
          <div class="nav-right nav-menu">
            <nuxt-link to="/" class="nav-item is-active">Home</nuxt-link>
            <nuxt-link to="/help" class="nav-item">Help</nuxt-link>
            <span class="nav-item">
              <a class="button is-info is-inverted">
                <span>Login</span>
              </a>
            </span>
          </div>
        </div>
      </header>
    </div>
  </section>
</template>
