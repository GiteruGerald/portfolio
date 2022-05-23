<template>
    <v-app style="{background: $vuetify.theme.themes.dark.background}">
    <NavBar />
      </v-app>
</template>

<script>
import NavBar from '@/components/NavBar.vue'

  export default {
    name: 'HomeView',

    components: {
      NavBar,
    },
  
        NavBar}
</script>
