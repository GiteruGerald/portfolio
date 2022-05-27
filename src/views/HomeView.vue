<template>
    <v-app id="home" :style="{background: $vuetify.theme.themes.dark.background}">
      <NavBar />
        <v-container fluid>
          <v-row>
              <v-col cols="6">
                <v-img src="gerryJ.black.jpg" contain max-height="500"></v-img>
              </v-col>
              <v-col cols="6">
                <h5 class="red--text text-darken-4 top"> Hello I'm Gerry</h5>
                <h1 class="white--text">Software Engineer</h1>
                <p class="grey--text">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. <br /> Suscipit temporibus quis
                   alias nihil? Consequuntur deserunt modi maiores 
                   obcaecati necessitatibus quam quas autem! <br />Ab praesentium nam adipisci obcaecati 
                   optio aspernatur voluptates?
                </p>
                <v-btn tile color="#a71210" dark>About Me</v-btn>
              </v-col>
          </v-row>
        </v-container>
      </v-app>
</template>

<script>
import NavBar from '@/components/NavBar.vue'

  export default {
    name: 'HomeView',

    components: {
      NavBar,
    },
  
        NavBar}
</script>
<style scoped>
.top{
  margin-top: 100px
}
.topInverse{
  margin-top: -250px;
}
.topTolbar{ 
  margin-top: 100px;
  text-align: center;
}
.first{ 
  width: 100px;
  height: 610px;
  background: linear-gradient(
    to right,
    #101010,
    #101010 50%,
    #111111 50%,
    #111111 50%,

  );
  text-align: center;
  padding: 2rem 2rem;
}
.second{ 
  width: 100%;
  height: 400px;
  background: #101010;
  text-align: center;
  padding: 2rem 2rem;
}
.secondChild{
  display: inline-block;
  background-color: #1e1e1e;
  padding: 2 rem 2 rem;
  vertical-align: middle;
  text-align: left;
  margin-top: 250px;
}
.child{ 
  display: inline-block;
  padding: 2rem 2rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
}
.bgColor1{ 
  background-color: #1e1e1e;
}
.bgColor2{ 
  background-color: #ce1d2a;
}
.child1{ 
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  margin-right: 5px;
  width: 240px;
}
.child2{ 
  display: inline-block;
  width: 245px;
  vertical-align: middle;
}
.mRight{ 
  margin-right: 8px;
}
.mButton{ 
  margin-bottom: 8px;
}
.padding{ 
  padding: 8px 0px 0px;
}
</style>
