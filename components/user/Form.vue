<template lang='pug'>
form(action='/api/users', method='post')
  .field
    label.label Username
    p.control.has-icons-left.has-icons-right
      input.input.is-success(type='text' value='')
      span.icon.is-small.is-left
        i.fa.fa-user
      span.icon.is-small.is-right
        i.fa.fa-check
    p.help.is-success This username is available
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
    label.label Password Confirmation
    p.control.has-icons-left.has-icons-right
      input.input.is-success(type='password' value='')
      span.icon.is-small.is-left
        i.fa.fa-key
      span.icon.is-small.is-right
        i.fa.fa-check
    p.help.is-success This password is available
  button.button.is-large(type='submit' name='action' value='submit') Submit
</tmplate>
