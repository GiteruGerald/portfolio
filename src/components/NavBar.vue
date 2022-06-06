<template>
    <v-app-bar app dark flat class="px-8">
        <v-btn icon>
            <v-icon color="#A71210">fas fa-dragon</v-icon>
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn text @click="scroll('home')">Home</v-btn>
        <v-btn text @click="scroll('about')">About</v-btn>
        <v-btn text @click="scroll('projects')">Projects</v-btn>
        <v-btn text @click="scroll('contact')">Contact</v-btn>
    </v-app-bar>
</template>

<script>
    export default {
        methods:{
            scroll(refName){
                const element = document.getElementById(refName);
                element.scrollIntoView({behavior: "smooth"});
            }
        },
    }
</script>
