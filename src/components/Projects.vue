<template>
    <v-row >
            <v-container class="pa-4 text-center">
                <h2 class="white--text">FEATURED PROJECTS</h2>
                <v-row class="fill-height mt-5" align="center" justify="center">
                    <template v-for="(item, i) in items">
                        <v-col :key="i" cols="12" md="4">
                        <v-hover v-slot="{ hover }">
                            <v-card :elevation="hover ? 12 : 2" :class="{ 'on-hover': hover }">
                            <v-img :src="item.img" height="225px">
                                <v-card-title class="text-h6 white--text">
                                <v-row class="fill-height flex-column" justify="space-between">
                                    <div class="align-self-center mt-10">
                                        <a :href="item.glink" target="_blank" rel="noopener noreferrer">

                                            <v-btn v-for="(icon, index) in icons" :key="index" :class="{ 'show-btns': hover }" 
                                    :color="transparent" icon >
                                        <v-icon :class="{ 'show-btns': hover }" :color="transparent" >
                                        {{ icon }}
                                        </v-icon>
                                    </v-btn>
                                        </a>
                                    </div>
                                </v-row>
                                </v-card-title>
                            </v-img>
                            <v-card-title>{{ item.title }}</v-card-title>
                            <v-divider></v-divider>
                            <v-card-subtitle> {{ item.text }} </v-card-subtitle>
                            </v-card>
                        </v-hover>
                        </v-col>
                    </template>
                </v-row>
  </v-container>

    </v-row>
</template>

<script>
    import bugtraq from '../assets/bugtraq.png';
    import fbars from '../assets/5bars.png';
    import portfolio from '../assets/portfolio.png';
    export default {
        data: () => ({
      icons: ['mdi-github'],
      items: [
        {
          title: 'BugTraq',
          text: `A bug tracking system of reported software bugs for use in the QA world`,
          img: bugtraq,
          glink: "https://github.com/GiteruGerald/BugTraq"
        },
        {
          title: 'FiveBars',
          text: 'A landing page of the "Five Bars Networks" company that is a regional broadband provider in Kenya',
          img: fbars,
          glink: "https://5bars.co.ke"
        },
        {
          title: 'Portfolio',
          text: 'A portfolio website to showcase my skills and recent projects.',
          img: portfolio,
          glink:"https://github.com/GiteruGerald/portfolio"
        },
      ],
      transparent: 'rgba(255, 255, 255, 0)',
    }),
    }
</script>

<style lang="scss" scoped>
.projects_div{
    width: 100%;
    text-align: center;
}
.v-card {
  transition: opacity .4s ease-in-out;
}

.v-card:not(.on-hover) {
  opacity: 0.6;
 }

.show-btns {
  color: rgba(255, 255, 255, 1) !important;
}

</style>