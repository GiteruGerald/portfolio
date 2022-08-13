<template>
  <v-app
    :style="{ background: $vuetify.theme.themes.dark.background }"
  >
  <NavBar/>
  <v-container fluid>
    <!-- Intro -->
      
        <intro/>
      
    <!-- About -->
        <Skills/>
    <!-- Projects -->
      <v-row>

      </v-row>
    <!-- Contact -->
      <v-row>

      </v-row>
  </v-container>
  </v-app>
</template>

<script>
import NavBar from '@/components/NavBar.vue';
import Intro from '@/components/Intro.vue';
import Skills from '@/components/Skills.vue';

  export default {
    components:{
    NavBar,
    Intro,
    Skills
}
  }
</script>

<style lang="scss" scoped>

</style>
