<template>
    <v-row >
            <v-container class="pa-4 text-center">
                <h2 class="white--text">FEATURED PROJECTS</h2>
                <v-row class="fill-height mt-5" align="center" justify="center">
                    <template v-for="(item, i) in items">
                        <v-col :key="i" cols="12" md="4">
                        <v-hover v-slot="{ hover }">
                            <v-card :elevation="hover ? 12 : 2" :class="{ 'on-hover': hover }">
                            <v-img :src="item.img" height="225px" contain>
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
  import images from '@/constants/images';
    export default {
        data: () => ({
      icons: ['mdi-github'],
      items: [
        {
          title: 'BugTraq',
          text: `A bug tracking system of reported software bugs for use in the QA world`,
          img: images.bugtraq,
          glink: "https://github.com/GiteruGerald/BugTraq"
        },
        {
          title: 'FiveBars',
          text: 'A landing page of the "Five Bars Networks" company that is a regional broadband provider in Kenya',
          img: images.fbars,
          glink: "https://5bars.co.ke"
        },
        {
          title: 'Portfolio',
          text: 'A portfolio website to showcase my skills and recent projects.',
          img: images.portfolio,
          glink:"https://github.com/GiteruGerald/portfolio"
        },
        {
          title: 'Weather App',
          text: 'Coding Challenge of a weather forecast that consumes an API and returns Hourly Weather results',
          img: images.weather,
          glink:"https://github.com/GiteruGerald/weather-app-vue"
        },
        {
          title: 'GreenSett Logistics',
          text: 'A landing page of the "GreenSett Logistics" company that is a logistics provider in Kenya',
          img: images.greensett,
          glink:"https://greensett.com"
        },
        {
          title: 'Survey Full Stack Application',
          text: 'Open source project to build many surveys with numerous choices and receive responses. ',
          img: images.survey,
          glink:"https://github.com/GiteruGerald/laravue-survey"
        },
      ],
      // transparent: 'rgba(255, 255, 255, 0)',
      transparent: 'rgba(245, 40, 145, 0.8)',
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