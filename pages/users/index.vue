<template>
  <section class="section">
    <div class="container">
      <h1>All users</h1>

      <!--<%= will_paginate %>-->

      <ul class="users">
        <li v-for="user in users">
          {{ user.name }}
        </li>
      </ul>

      <!--<%= will_paginate %>-->
    </div>
  </section>
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
