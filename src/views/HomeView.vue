<template>
  <v-app
    :style="{ background: $vuetify.theme.themes.dark.background }"
  >
  <NavBar/>
  <v-container fluid>
    <!-- Intro -->
      
        <intro id="home"/>
      
    <!-- About -->

        <Skills id="skills"/>
    <!-- Projects -->
        <Projects id="projects"/>
    <!-- Contact -->
      
        <Contact id="contact"/>
      <!-- Footer -->
      <Footer/>
  </v-container>
  </v-app>
</template>

<script>
import NavBar from '@/components/NavBar.vue';
import Intro from '@/components/Intro.vue';
import Skills from '@/components/Skills.vue';
import Footer from '@/components/Footer.vue';
import Projects from '@/components/Projects.vue';
import Contact from '@/components/Contact.vue';

  export default {
    components:{
    NavBar,
    Intro,
    Skills,
    Footer,
    Projects,
    Contact
}
  }
</script>

<style>

</style>
