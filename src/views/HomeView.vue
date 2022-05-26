<template>
    <v-app :style="{background: $vuetify.theme.themes.dark.background}">
      <NavBar />
        <v-container>
          <v-row>
              <v-col cols="6">
                <v-img src="gerryJ.black.jpg" contain max-height="500"></v-img>
              </v-col>
          </v-row>
        </v-container>
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
