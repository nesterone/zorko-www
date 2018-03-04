<template>
  <v-app light>
    <v-toolbar class="white">
      <v-avatar>
        <img src="~/assets/logo.png" alt="Zorko">
      </v-avatar>
    </v-toolbar>
    <main>
      <nuxt/>
    </main>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'apps', title: 'Welcome', to: '/' },
          { icon: 'bubble_chart', title: 'Inspire', to: '/inspire' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Zorko'
      }
    }
  }
</script>
