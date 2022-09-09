<template>
    <v-row>
        <div class="flex" >
            <v-col cols="6" xl="6" md="6" xs="8" class="top">
               <h2 class="text-darken-8 ">
                    <span style="color:#72DAEF">Hi there👋🏽, I'm Gerald Giteru</span>
                </h2>
                <h1 class="white--text">Software Engineer</h1>
                <p class="grey--text">
                 Here to help you develop your solutions and have a taste of the Web-presence that is growing each and everyday.
                </p>
                <a href="https://drive.google.com/file/d/1-XGZatEvvbM0VxyugfBnMKD9QvKwvqqT/view?usp=sharing"
                 style="text-decoration:none"
                 target="blank"
                 class="resume-link">
                    <v-btn tile color="#72DAEF" dark>Resume/CV
                        <v-icon>mdi-download-box</v-icon>
                    </v-btn>    
                </a>
          
                </v-col> 
            <v-col cols="6" xl="6" md="6" xs="0" class="hidden-xs-only">
                <v-img src="gerryJ.black.jpg" md="20" max-height="500" contain>
                </v-img>  
            </v-col>
        </div>
        
        
    </v-row>
</template>

<script>
    export default {
        name:"Intro",
        methods:{
            scroll(refName){
                const element = document.getElementById(refName);
                element.scrollIntoView({behavior: "smooth", block: "start", inline: "nearest"});
            }
        },
    }
</script>

<style lang="scss" scoped>

.top {
  margin-top: 150px;
  margin-left: 40px;
}
.flex{
    display: flex;
    margin-left: 20px;
     min-height: 100vh;
}
.resume-link{
    margin-right: 30ex;
}
</style>
    
}

</style>