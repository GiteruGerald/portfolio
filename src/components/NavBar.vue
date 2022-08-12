<template>
    <v-app-bar app dark flat class="px-8">
        <v-btn icon>
            <v-img src="GJ-Logo.png" contain max-height="65"></v-img>

            <v-icon color="#72DAEF">fas fa-dragon</v-icon>
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn text @click="scroll('home')">Home</v-btn>
        <v-btn text @click="scroll('about')">About</v-btn>
        <v-btn text @click="scroll('projects')">Projects</v-btn>
        <v-btn text @click="scroll('contact')">Contact</v-btn>
        <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
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
