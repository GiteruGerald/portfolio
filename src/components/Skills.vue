  <template>
    <v-row>
      <!-- Before -->
        <div class="skills_div">
          <h2 class="white--text ml-4">SKILLS & EXPERIENCES</h2>
          <p class="white--text mt-2">
              Languages & Frameworks
            </p>
          <!-- App Badges -->
          <v-col cols="12">
            <v-row>
              <v-col cols="6" lg="6" md="4" sm="3" xs="12">
                <Timeline/>
  
              </v-col >
              <v-spacer></v-spacer>
              <v-col cols="6" lg="6" md="4" sm="3" xs="12">
  
                <AppBadges/>
              </v-col>
            </v-row>
            
          </v-col>
          <v-col cols="12">

            <v-col cols="3" md="3" sm="3" xs="12" class="child mt-7 " style="background-color:#1e1e1e">
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
            </v-col>

            <v-col cols="3" md="3" sm="3" xs="12" class="child" style="background-color:#72DAEF">
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
            </v-col>
            <v-col cols="3" md="3" sm="3" xs="12" class="child" style="background-color:#1e1e1e">
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
            </v-col>
          </v-col>
              

              </div>
    </v-row>
</template>

<script>
import AppBadges from './AppBadges.vue';
import Timeline from './Timeline.vue';
    export default {
        components:{
    AppBadges,
    Timeline
}
    }
</script>

<style lang="scss" scoped>
.child {
  display: inline-block;
  padding: 2rem 1rem;
  // vertical-align: middle;
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
  // padding: 2rem 2rem;
}


</style>