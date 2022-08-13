<template>
  <v-app
    :style="{ background: $vuetify.theme.themes.dark.background }"
  >
    <NavBar />
    <v-container fluid>
      <div id="home">
        <v-row>
          <v-col cols="6">
            <v-img src="gerryJ.black.jpg" contain max-height="500"></v-img>
          </v-col>
          <v-col cols="6">
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
          <v-col cols="12" class="padd">
            <div class="first" id="about">
              <v-row>
                <v-col lg="12" md="9">
                  <div class="child bgColor1">
                    <v-icon color="#72DAEF" x-large class="ml-3">
                      mdi-palette-swatch
                    </v-icon>
                    <h3 class="white--text ml-3 mt-4">Full Stack Web Dev</h3>
                    <p class="grey--text ml-3 mt-6">
                      Lorem ipsum dolor sit amet consectetur adipisicing
                      elit.<br />
                      Suscipit voluptas ex, non vero nostrum in<br />,
                    </p>
                    <v-btn color="#72DAEF" dark text>
                      know more
                      <v-icon right>mdi-arrow-right</v-icon>
                    </v-btn>
                  </div>
                  <div class="child bgColor2">
                    <v-icon x-large class="ml-3" dark>mdi-shopping</v-icon>
                    <h3 class="white--text ml-3 mt-4">Product Design</h3>
                    <p class="grey--text ml-3 mt-6">
                      Lorem ipsum dolor sit amet consectetur adipisicing
                      elit.<br />
                      Suscipit voluptas ex, non vero nostrum in<br />,
                    </p>
                    <v-btn dark text>
                      know more
                      <v-icon right>mdi-arrow-right</v-icon>
                    </v-btn>
                  </div>
                  <div class="child bgColor1">
                    <v-icon color="#72DAEF" x-large class="ml-3"
                      >mdi-book-open-page-variant</v-icon
                    >
                    <h3 class="white--text ml-3 mt-4">Branding</h3>
                    <p class="grey--text ml-3 mt-6">
                      Lorem ipsum dolor sit amet consectetur adipisicing
                      elit.<br />
                      Suscipit voluptas ex, non vero nostrum in<br />,
                    </p>
                    <v-btn color="#72DAEF" dark text>
                      know more
                      <v-icon right>mdi-arrow-right</v-icon>
                    </v-btn>
                  </div>
                </v-col>
                <v-col class="mt-10">
                  <div class="child1">
                    <h1 class="text-darken-4 mt-4 number">12</h1>
                    <h3 class="white--text mt-4">Years Experience</h3>
                  </div>
                  <div class="child2 mRight">
                    <v-row>
                      <v-col cols="12" class="childCol">
                        <div class="child2 mButton padding bgColor1">
                          <h1 class="text--darken-4" style="color:#72DAEF">50+</h1>
                          <p class="grey--text">Clients</p>
                        </div>
                      </v-col>
                      <v-col cols="12" class="childCol">
                        <div class="child2 padding bgColor1">
                          <h1 class="text--darken-4" style="color:#72DAEF">122+</h1>
                          <p class="grey--text">Completed Projects</p>
                        </div>
                      </v-col>
                    </v-row>
                  </div>
                  <div class="child2">
                    <v-row>
                      <v-col cols="12" class="childCol">
                        <div class="child2 mButton padding bgColor1">
                          <h1 class="text--darken-4" style="color:#72DAEF">08</h1>
                          <p class="grey--text">Years Experience</p>
                        </div>
                      </v-col>
                      <v-col cols="12" class="childCol">
                        <div class="child2 padding bgColor1">
                          <h1 class="text--darken-4" style="color:#72DAEF">10</h1>
                          <p class="grey--text">Achievements</p>
                        </div>
                      </v-col>
                    </v-row>
                  </div>
                </v-col>
              </v-row>
            </div>
          </v-col>
          <v-col md="12" offset-md="10" id="projects">
            <h4 class="white--text">FEATURED PROJECTS</h4>
            <p class="grey-text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
          </v-col>
          <v-col md="3" class="text-end">
            <v-btn tile color="#72DAEF" dark>View All</v-btn>
          </v-col>
          <v-col md="3" offset-md="3">
            <v-card
              tile
              class="pa-2 py-12"
              outlined
              height="250px"
              color="#1e1e1e"
            >
              <v-img src="1.png" contain></v-img>
            </v-card>
          </v-col>
          <v-col md="3">
            <v-card
              tile
              class="pa-2 py-12"
              outlined
              height="250px"
              color="#1e1e1e"
            >
              <v-img src="1.png" contain></v-img>
            </v-card>
          </v-col>
          <v-col md="3" offset-md="3">
            <v-btn color="white" dark text class="ml-n4"> BUGTRAQ </v-btn><br />

            <v-btn color="#72DAEF" dark text class="ml-n4">
              know more
              <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
          </v-col>
          <v-col md="3">
            <v-btn color="white" dark text class="ml-n4">
              WATER BILLING SYSTEM </v-btn
            ><br />

            <v-btn color="#72DAEF" dark text class="ml-n4">
              know more
              <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
          </v-col>
          <v-col md="3" offset-md="3">
            <v-card
              class="pa-2 py-12"
              outlined
              tile
              height="250px"
              color="#1E1E1E"
            >
              <v-img src="1.png" contain max-height=""></v-img>
            </v-card>
          </v-col>
          <v-col md="3">
            <v-card
              class="pa-2 py-12"
              outlined
              tile
              height="250px"
              color="#1E1E1E"
            >
              <v-img src="1.png" contain max-height=""></v-img>
            </v-card>
          </v-col>
          <v-col md="3" offset-md="3">
            <v-btn color="white" dark text class="ml-n4"> AAE IdeaPro </v-btn
            ><br />

            <v-btn color="#72DAEF" dark text class="ml-n4">
              know more
              <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
          </v-col>
          <v-col md="3">
            <v-btn color="white" dark text class="ml-n4"> Mozaik </v-btn><br />
            <v-btn color="#72DAEF" dark text class="ml-n4">
              know more
              <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
          </v-col>
          <v-col cols="12" class="padd topInverse">
            <div class="second">
              <div class="secondChild1" id="contact">
                <v-row>
                  <v-col cols="7">
                    <h1 class="white--text">
                      Let's work together on<br />your next project
                    </h1>
                    <p class="grey--text">
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Eius nesciunt ducimus natus <br />
                    </p>
                  </v-col>
                  <v-col cols="5">
                    <v-btn tile color="#72DAEF" dark class="mt-16"
                      >Contact</v-btn
                    >
                  </v-col>
                </v-row>
              </div>
            </div>
            <v-toolbar class="topTolbar" color="#111111" dark flat>
              <div
                style="
                  position: absolute;
                  margin-left: auto;
                  margin-right: auto;
                  left: 0;
                  right: 0;
                  text-align: center;
                "
              >
                <v-btn text>Home</v-btn>
                <v-btn text>Project</v-btn>
                <v-btn text>about</v-btn>
                <v-btn text> contact</v-btn>
              </div>
            </v-toolbar>
          </v-col>
        </v-row>
      </div>
    </v-container>
    <FooterBar />
  </v-app>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import FooterBar from "@/components/Footer.vue";
export default {
  name: "HomeView",

  components: {
    NavBar,
    FooterBar,
  },
};
</script>
<style scoped>
.top {
  margin-top: 180px;
}
.topInverse {
  margin-top: -250px;
}
.topTolbar {
  margin-top: 100px;
  text-align: center;
}
.first {
  width: 100%;
  height: 610px;
  background: linear-gradient(
    to right,
    #181818,
    #181818 50%,
    #111111 50%,
    #111111 50%
  );
  text-align: center;
  padding: 2rem 2rem;
}
.second {
  width: 100%;
  height: 400px;
  background: #181818;
  text-align: center;
  padding: 2rem 2rem;
}
.secondChild1 {
  display: inline-block;
  background-color: #1e1e1e;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-top: 250px;
}
.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
}
.bgColor1 {
  background-color: #1e1e1e;
}
.bgColor2 {
  background-color: #72DAEF;
}
.child1 {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  margin-right: 5px;
  width: 240px;
  color: #72DAEF;
}
.child2 {
  display: inline-block;
  width: 245px;
  vertical-align: middle;
  color: #72DAEF;

}
.mRight {
  margin-right: 8px;
}
.mButton {
  margin-bottom: 8px;
}
.padding {
  padding: 8px 0;
}
.col-12.padd {
  padding: 12px 0 !important;
}
.col-12.childcol {
  padding: 0 !important;
  
}
h1.number {
  font-size: 50px;
  font-weight: bold;
}
</style>
