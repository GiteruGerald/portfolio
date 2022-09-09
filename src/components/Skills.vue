  <template>
    <v-row>
      <!-- Before -->
        <div class="skills_div">
          <h2 class="white--text ml-4">SKILLS & EXPERIENCES</h2>
          <p class="white--text mt-2">
              Languages & Frameworks I've worked with
            </p>
          <!-- App Badges -->
                <v-col cols="12" lg="12" md="9" sm="9" xs="12">
                    <div class="box-flex">
                      <AppBadges/>
                    </div>
                    <div>
                      <v-container class=" text-center">
                          <v-row class="fill-height mt-5" justify="center">
                              <template v-for="(item, i) in items">
                                  <v-col :key="i" cols="12" md="4">
                                      <v-card :color="item.color">
                                      
                                          <v-card-title class="text-h6 white--text">
                                          <v-row class="fill-height flex-column" justify="space-between">
                                              <div class=" mt-10">
                                                  <v-icon x-large :color="item.iconColor" >
                                                  {{ item.icon }}
                                                  </v-icon>
                                              </div>
                                          </v-row>
                                          </v-card-title>
                                      <v-card-title :class="item.textColor"> {{ item.title   }}</v-card-title>
                                      <v-divider></v-divider>
                                      <v-card-subtitle > {{ item.text }} </v-card-subtitle>
                                      </v-card>
                                  </v-col>
                              </template>
                          </v-row>
                   </v-container>
                    </div>
                   

                </v-col>
          
              

              </div>
    </v-row>
</template>

<script>

import AppBadges from './AppBadges.vue';
    export default {
        components:{ AppBadges },
        data:()=>({
          items:[
            {
              title:"Software Development",
              icon:"mdi-server",
              color:"black",
              textColor:"white--text",
              iconColor:"#72DAEF"
            },
            {
              title:"DevOps",
              icon:"mdi-microsoft-azure-devops",
              color:"#72DAEF",
              textColor:"white--text",
              iconColor:"white"
            },
            {
              title:"System Audit",
              icon:"mdi-book-search",
              color:"black",
              textColor:"white--text",
              iconColor:"#72DAEF"
            },
           
          ]
        }),
       
    }
</script>

<style lang="css" scoped>

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
  min-height: 80vh;
  padding: 2rem 2rem;
}


</style>