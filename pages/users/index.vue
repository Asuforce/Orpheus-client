<template lang="pug">
  section.hero
    .hero-body
      .container
        h1.title All users

        //- <%= will_paginate %>

        ul
          li(v-for="user in users")
            user-field
              img(slot='image', v-bind:src="user.img", v-bind:alt="user.name")
              p.title.is-4(slot='name') {{ user.name }}
              p.subtitle.is-6(slot='id') @{{ user.name }}

        //- <%= will_paginate %>
</template>

<script>
import axios from 'axios'
import UserField from '~components/user/Field.vue'

export default {
  components: {
    UserField
  },
  asyncData () {
    return axios.get('http://localhost:3001/api/users').then(res => res.data)
  },
  head () {
    return {
      title: 'All users'
    }
  }

}
</script>
