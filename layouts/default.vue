<template>
  <div>
    <custom-header/>
    <div class="container">
      <nuxt/>
    </div>
    <custom-footer/>
  </div>
</template>


<script>
import CustomHeader from '~components/Header.vue'
import CustomFooter from '~components/Footer.vue'
export default {
  name: 'default',
  components: {
    CustomHeader,
    CustomFooter
  }
}
</script>
