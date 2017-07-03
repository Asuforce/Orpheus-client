<template lang='pug'>
div
  .card-content
    .media
      .media-left
        figure.image.is-50x50
          slot(name='image')
      .media-content
        slot(name='name')
        slot(name='id')

//- - if current_user.admin? && !current_user?(user)
//-   |  |
//-   = link_to "delete", user, method: :delete, data: { confirm: "You sure?" }
</template>
