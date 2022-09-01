  <template>
    <v-row>
        

      <!-- Before -->
        <div class="skills_div">
          <h2 class="white--text ml-4">SKILLS & EXPERIENCES</h2>
          <p class="white--text mt-2">
              Languages & Frameworks I've worked with
            </p>
          <!-- App Badges -->
            <v-parallax src="https://cdn.vuetifyjs.com/images/parallax/material.jpg" max-height="100px" contain>
                <v-col cols="12" lg="12" md="9" sm="9" xs="12">
                    <div class="mt-10">
                      <AppBadges/>
                        </div>
                    <v-col cols="12">
                            <v-col cols="12" md="12" sm="12" xs="12" class="child mt-7 " style="background-color:#1e1e1e">
                              <v-icon color="#72DAEF" x-large class="ml-3">mdi-server</v-icon>
                              <p class="white--text ml-3 mt-4">Software-dev</p>
                              
                            </v-col>

                            <v-col cols="12" md="12" sm="12" xs="12" class="child mt-7 " style="background-color:#72DAEF">
                              <v-icon x-large class="ml-3" dark>mdi-microsoft-azure-devops</v-icon>
                              <h3 class="white--text ml-3 mt-4">Devops</h3>
                            
                            </v-col>
                            <v-col cols="12" md="12" sm="12" xs="12" class="child mt-7 mb-10" style="background-color:#1e1e1e">
                              <v-icon color="#72DAEF" x-large class="ml-3">mdi-book-search</v-icon>
                              <h3 class="white--text ml-3 mt-4">Systems Audit</h3>
                              
                            </v-col>
                        </v-col>
                        
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
  display: inline-flex;
  padding: 1rem 1rem;
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


</style>