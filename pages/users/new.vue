<template lang="pug">
  section.hero
    .hero-body
      .container
        //- provide(:button_text, "Create my account")
        h1.title Sign up
        .row
          .col-md-6.col-md-offset-3
            user-form
</template>

<script>
import UserForm from '~components/user/Form.vue'

export default {
  components: {
    UserForm
  },
  head () {
    return {
      title: 'Sign up'
    }
  }
}
</script>
