<template>
    <v-row>
        <div class="second">
                  <div class="secondChild1" >
                    <v-row>
                      <v-col cols="6" lg="7" md="12" sm="12" xs="12">
                        <h1 class="white--text">
                          Have a question or want to say hello? 
                        </h1>
                        <p class="grey--text hidden-sm-and-down">
                          Let's talk over coffee on your next project 😊
                        </p>
                        <br>
                        <a href="mailto:geraldgiteru@gmail.com" style="text-decoration:none">  
                          <v-btn tile color="#72DAEF" dark>
                            <v-spacer></v-spacer>
                            <v-icon>fas fa-envelope</v-icon>
                              <!-- <p class="grey--text"> -->
                                  geraldgiteru@gmail.com
                                  <!-- </p> -->
                            </v-btn>
                          </a>
                          <br>
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
  // padding: 2rem 2rem;
  margin-top: 40px;
}
.secondChild1 {
  display: inline-block;
  width: 80%;
  background-color: #1e1e1e;
  padding: 2rem 1rem;
  vertical-align: baseline;
  text-align: left;
  
}
.flex{
  display: flexbox;
}
</style>