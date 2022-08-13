<template>
    <v-app-bar app dark flat class="px-8"> 
       
       <v-toolbar dense>
            <v-btn icon>
                    <v-img src="GJ-Logo.png" contain max-height="65"></v-img>

                </v-btn>
                <v-spacer></v-spacer>
                    <router-link to="/about">About</router-link>
                <v-toolbar-items class="hidden-xs-only">
                    <v-btn text @click="scroll('home')">Home</v-btn>
                    <v-btn text @click="scroll('about')">About</v-btn>
                    <v-btn text @click="scroll('projects')">Projects</v-btn>
                    <v-btn text @click="scroll('contact')">Contact</v-btn>
                </v-toolbar-items>
    </v-toolbar>
         <div class="hidden-sm-and-up">
            <v-menu transition="slide-x-transition" bottom right>
              <template v-slot:activator="{ on }">
                <v-app-bar-nav-icon v-on="on"></v-app-bar-nav-icon> 
              </template>

              <v-list dense class="responsiveMenu">
                <v-list-item>
                  <v-list-item-title @click="scroll('home')">HOME</v-list-item-title>
                    
                  <v-list-item-title>
                    <v-btn text @click="scroll('skills')">Skills</v-btn>
                  </v-list-item-title>
                  <v-list-item-title>
                    <v-btn text @click="scroll('projects')">Projects</v-btn>
                  </v-list-item-title>
                  <v-list-item-title>
                    <v-btn text @click="scroll('contact')">Contact</v-btn>
                  </v-list-item-title>
                </v-list-item>
              </v-list>
            </v-menu>
         </div>
     </v-app-bar>
</template>

<script>
    export default {
        data: () => ({ drawer: null }),
        methods:{
            scroll(refName){
                const element = document.getElementById(refName);
                element.scrollIntoView({behavior: "smooth"});
            }
        },
    }
</script>
