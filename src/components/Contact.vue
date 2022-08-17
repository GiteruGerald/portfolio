<template>
    <v-row>
        <div class="second">
                  <div class="secondChild1" >
                    <v-row>
                      <v-col cols="7" lg="7" md="4" sm="3" xs="3">
                        <h1 class="white--text">
                          Have a question or want to say hello? 
                        </h1>
                        <p class="grey--text">
                          Let's talk over coffee on your next project 😊
                        </p>
                      </v-col>
                      <v-col cols="5" lg="5" md="6" sm="9" xs="9">
                        <a href="mailto:geraldgiteru@gmail.com" style="text-decoration:none">  
                          <v-btn tile color="#72DAEF" dark class="mt-16">
                            <v-spacer></v-spacer>
                            <v-icon>fas fa-envelope</v-icon>
                              <!-- <p class="grey--text"> -->
                                  geraldgiteru@gmail.com
                                  <!-- </p> -->
                            </v-btn>
                          </a>
                          
                        <a href="tel: +254718889118" style="text-decoration:none">  
                          <v-btn tile color="#72DAEF" dark class="mt-4">
                            <v-icon>fas fa-mobile-screen</v-icon>
                            <v-spacer></v-spacer>
                              <!-- <p class="grey--text"> -->
                                  +254718 889 118
                                  <!-- </p> -->
                            </v-btn>
                          </a>
                          
                      </v-col>
                    </v-row>
                  </div>
                </div>
    </v-row>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.second {
  width: 100%;
  height: 400px;
  background: #181818;
  text-align: center;
  padding: 2rem 2rem;
  margin-top: 40px;
}
.secondChild1 {
  display: inline-block;
  background-color: #1e1e1e;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  
}

</style>