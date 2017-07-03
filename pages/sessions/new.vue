<template lang="pug">
  section.hero
    .hero-body
      .container
        h1.title Login
        .row
          .col-md-6.col-md-offset-3
            form(action='/api/login', method='post')
              .field
                label.label Email
                p.control.has-icons-left.has-icons-right
                input.input.is-danger(type='text' value='')
                span.icon.is-small.is-left
                  i.fa.fa-envelope
                span.icon.is-small.is-right
                  i.fa.fa-warning
              p.help.is-danger This email is invalid
              .field
                label.label Password
                p.control.has-icons-left.has-icons-right
                  input.input.is-success(type='password' value='')
                  span.icon.is-small.is-left
                    i.fa.fa-key
                  span.icon.is-small.is-right
                    i.fa.fa-check
                p.help.is-success This password is available
              .field
                button.button.is-large(type='submit' name='action' value='submit') Submit
</template>

<script>
</script>
