<template>
    <v-row>
        <div class="flex">
            <v-col cols="6" md="6" xs="8">
               <h2 class="text-darken-8 top">
                    <span style="color:#72DAEF">Hi there👋🏽, I'm Gerald Giteru</span>
                </h2>
                <h1 class="white--text">Software Engineer</h1>
                <p class="grey--text">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. <br />
                Suscipit temporibus quis alias nihil? Consequuntur deserunt modi
                maiores obcaecati necessitatibus quam quas autem! <br />Ab
                praesentium nam adipisci obcaecati optio aspernatur voluptates?
                </p>
                <v-btn tile color="#72DAEF" dark>About Me</v-btn>    
          
                </v-col> 
            <v-col cols="6" md="6" xs="0" class="hidden-xs-only">
                <v-img src="gerryJ.black.jpg" md="20" max-height="500" contain>
                </v-img>  
            </v-col>
        </div>
        
        
    </v-row>
</template>

<script>
    export default {
        name:"Intro"
    }
</script>

<style lang="scss" scoped>
.top {
  margin-top: 80px;
}
.flex{
    display: flex;
}

</style>