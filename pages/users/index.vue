<template lang="pug">
  section.hero
    .hero-body
      .container
        h1.title All users

        //- <%= will_paginate %>

        ul
          li(v-for="user in users") {{ user.name }}

        //- <%= will_paginate %>
</template>

<script>
import axios from 'axios'

export default {
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
