  <template>
    <v-row>
        

      <!-- Before -->
        <div class="skills_div">
          <h2 class="white--text ml-4">SKILLS & EXPERIENCES</h2>
          <p class="white--text mt-2">
              Languages & Frameworks I've worked with
            </p>
          <!-- App Badges -->
            <v-parallax src="https://cdn.vuetifyjs.com/images/parallax/material.jpg" max-height="80px" contain>
                <v-col cols="12" lg="12" md="9" sm="9" xs="12">
                    <div class="skills-flex">
                      <AppBadges/>
                        </div>
                        <div class="box-flex">
                          <v-col cols="12">
                                  <v-col cols="4" md="4" sm="3" xs="3" class="child mt-7 " style="background-color:#1e1e1e">
                                    <v-icon x-large class="ml-1" color="#72DAEF" >mdi-server</v-icon>
                                    <span class="white--text mt-4 hidden-xs-only">Software-dev</span>
                                    
                                  </v-col>
      
                                  <v-col cols="4" md="4" sm="3" xs="3" class="child mt-7 " style="background-color:#72DAEF">
                                    <v-icon x-large class="ml-1" dark>mdi-microsoft-azure-devops</v-icon>
                                    <span class="white--text mt-4  hidden-xs-only">DevOps</span>
                                  
                                  </v-col>
                                  <v-col cols="4" md="4" sm="3" xs="3" class="child mt-7 mb-10" style="background-color:#1e1e1e">
                                    <v-icon  x-large class="ml-1" color="#72DAEF">mdi-book-search</v-icon>
                                    <span class="white--text mt-4 hidden-xs-only">Systems Audit</span>
                                    
                                  </v-col>
                              </v-col>
                        </div>
                        
                  <!-- <v-row> -->
                    <!-- <v-col cols="6" lg="6" md="4" sm="3" xs="12"> -->
                      <!-- <Timeline/> -->
        
                    <!-- </v-col > -->
                    <!-- <v-spacer></v-spacer> -->
                    <!-- <v-col cols="6" lg="6" md="4" sm="3" xs="12"> -->
        
                    <!-- </v-col> -->
                  <!-- </v-row> -->
                  
                </v-col>
            </v-parallax>
          
              

              </div>
    </v-row>
</template>

<script>

import AppBadges from './AppBadges.vue';
import Timeline from './Timeline.vue';
    export default {
        components:{ AppBadges, Timeline },
       
    }
</script>

<style lang="scss" scoped>
.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: baseline;
  text-align: left;
  margin-right: 3px;
}
.skills_div{
  width: 100%;
  background: linear-gradient(
    to right,
    #fffcfc,
    #181818 50%,
    #111111 50%,
    #111111 50%
  );
  text-align: center;
  min-height: 60vh;
  // padding: 2rem 2rem;
}
.skills-flex{
  // display:grid;
  // margin-bottom: 20ex;
  margin-top: 30ex;
}
.box-flex{
  margin-bottom: 30ex;
}

</style>