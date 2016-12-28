<template>
  <header>
    <nuxt-link class="button" v-for="link in navLinks" :to="link.path">
      {{link.text}}
    </nuxt-link>
  </header>
</template>

<script>
  export default {
    data () {
      return {
        navLinks: [
          {
            path: '/',
            text: 'Home'
          },{
            path: '/about',
            text: 'About'
          },{
            path: '/contact',
            text: 'Contact'
          },
        ]
      }
    }
  }
</script>
