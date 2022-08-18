<template>
    <v-footer dark padless>
        <v-card tile flat class="black white--text py-5 px-5 text-center" width="100%">
            <v-row>
                <v-col cols="12" sm="4">
                    <v-card-text class="pt-2">
                        <a href="https://github.com/GiteruGerald/" target="blank">
                            <v-btn class="mx-1 white--text" icon>
                                <v-icon size="24px">
                                    <!-- {{ icon }} -->
                                        fa-brands fa-github
                                </v-icon>
                                <v-spacer></v-spacer>
                            </v-btn>
                        </a>
                        <a href="https://www.linkedin.com/in/gerald-giteru/" target="blank">
                            <v-btn class="mx-1 white--text" icon>
                                <v-icon size="24px">
                                    <!-- {{ icon }} -->
                                        fa-brands fa-linkedin
                                </v-icon>
                            </v-btn>
                        </a>
                    </v-card-text>
                </v-col>
                <v-col cols="12" sm="4">
                    
                </v-col>
                <v-col cols="12" sm="4">
                    <v-card-text class="pt-2">
                        <p>Design and Developed by Gerald Giteru &copy;{{  new Date().getFullYear() }}</p> 
                        
                    </v-card-text>
                </v-col>
            </v-row>
        </v-card>
    </v-footer>
</template>

<script>
export default {
    name:"FooterBar",
    data:()=>({
        icons:["mdi-linkedin",
        "mdi-github"]
    }),
    setup () {
        

        return {}
    }
}
</script>

<style lang="scss" scoped>

</style>