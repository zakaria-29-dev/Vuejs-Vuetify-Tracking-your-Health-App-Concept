<template>
  <v-app :style="{background: $vuetify.theme.themes.light.background}">
    <v-layout row>
      <v-flex md8>
        <v-app :style="{background: $vuetify.theme.themes.dark.background}" class="rounded-tr-xl rounded-br-xl">
          <v-container>
              <v-row>
                <v-col cols="12" sm="12">
                  <v-app-bar color="rgba(0,0,0,0)" flat class="mx-8 mb-8 mt-3">
                    <v-text-field
                    prepend-icon="mdi-magnify"
                    color="teal"
                    placeholder="Search your symptoms"
                    flat
                    success 
                  ></v-text-field>
                  <v-spacer></v-spacer>
                   <v-chip
                    class="ma-2"
                    color="white" 
                  >
                    <v-icon left color="teal">
                      mdi-clock-time-nine
                    </v-icon>
                    14:02 AM Today Nov,19
                  </v-chip>
                  </v-app-bar>
                </v-col>
                <v-col cols="12" sm="12">
                  <v-card class="mx-12 rounded-tl-xl rounded-tr-xl rounded-bl-xl rounded-br-xl mt-n15" >
                  <v-list-item three-line>
                    <v-list-item-content class="pa-10">
        <v-list-item-title class="headline mb-1">
          Today <span class="teal--text">-10%</span> discount<br>
          on lung examinations
        </v-list-item-title>
        <v-list-item-subtitle>
          The package price includes: consultation<br>
          of a pulmonologist, spirography, cardiogram <span class="teal--text">></span>
        </v-list-item-subtitle>
      </v-list-item-content>

      <v-list-item-avatar
        tile
        size="150"
        class="pr-10"
        
      >
      <img src="lungs.png">
      </v-list-item-avatar>
    </v-list-item>

  </v-card>
                </v-col>
                <v-col cols="12" sm="12">
                  <v-card class="mx-12 rounded-tl-xl rounded-tr-xl rounded-bl-xl rounded-br-xl mt-n10">
                    <v-app-bar color="rgba(0,0,0,0)" flat class="ma-8">
                   <h5>Statistics of your health</h5>
                  <v-spacer></v-spacer>
                  <v-btn 
                  color="teal"
                      text
                      >2019  
                    <v-icon right>   
                      mdi-chevron-down
                    </v-icon>
                  </v-btn>
                   <v-btn color="teal" rounded dark depressed>Year</v-btn>
                   <v-btn text >Mounth</v-btn>
                  </v-app-bar>
                  <template>
                <v-sparkline
                  :value="value"
                  color="teal"
                  :smooth="radius || false"
                  :padding="padding"
                  :line-width="width"
                  :stroke-linecap="lineCap" 
                  :fill="fill"
                  :type="type"
                  :auto-line-width="autoLineWidth"
                  auto-draw
                ></v-sparkline>
                      </template>
                  </v-card>
                </v-col>
                <v-col cols="12" sm="6">
                    <v-card class="mx-12 rounded-tl-xl rounded-tr-xl rounded-bl-xl rounded-br-xl mt-n4" 
                    color="teal" dark >
                  <v-list-item three-line>
                    <v-list-item-content class="pa-2">
        <v-list-item-title class="headline mb-1">
          Heart rate <br>
          <h2>112 bpm</h2>
        </v-list-item-title>

      </v-list-item-content>

      <v-list-item-avatar
        tile
        size="150"
        class="pr-10"
        
      >
      <v-icon size="100">fas fa-heartbeat</v-icon>
      </v-list-item-avatar>
    </v-list-item>

  </v-card>
                </v-col>
                 <v-col cols="12" sm="6">
<v-card class="mx-12 rounded-tl-xl rounded-tr-xl rounded-bl-xl rounded-br-xl mt-n12" 
                      >
      
          <v-app-bar color="rgba(0,0,0,0)" flat class="ma-8">
                   <h5>Your activity</h5>
                  <v-spacer></v-spacer>
                   <v-btn color="teal" rounded dark depressed>Week</v-btn>
                   <v-btn text >Mounth</v-btn>
                  </v-app-bar>      
                  <v-progress-circular
                        rotate="360"
                        size="100"
                        width="15"
                        value="50"
                        color="teal"
                        class="mt-n5 ml-5 mb-2"
                      >
                       50
                      </v-progress-circular>
                      <v-progress-circular
                        rotate="360"
                        size="100"
                        width="15"
                        value="70"
                        color="red"
                        class="mt-n5 ml-2 mb-2"
                      >
                       70
                      </v-progress-circular>
                      <v-progress-circular
                        rotate="360"
                        size="100"
                        width="15"
                        value="80"
                        color="blue"
                        class="mt-n5 ml-2 mb-2"
                      >
                       80
                      </v-progress-circular>
                  </v-card>
                 </v-col>
              </v-row>
          </v-container>
        </v-app>
      </v-flex>
       <v-flex md4>
        <v-app :style="{background: $vuetify.theme.themes.light.background}">
          <v-container>
              <v-row>
                <v-col cols="12" sm="12">
                  <v-list two-line>
     
            <v-list-item
            >
              <v-list-item-avatar>
                <img src="https://cdn.vuetifyjs.com/images/lists/3.jpg">
              </v-list-item-avatar>
              <v-list-item-content>
                <v-list-item-title >Anastasia Turner</v-list-item-title>
                <v-list-item-subtitle class="teal--text">35 years, Houston</v-list-item-subtitle>    
              </v-list-item-content>
              <v-spacer></v-spacer>
                 <v-icon color="teal">mdi-menu</v-icon>
            </v-list-item>
        </v-list>
              </v-col>
              <v-col cols="12" md="4" >
                   <v-row>
                     <v-col cols="12" md="2">
                        <v-card height="50px" width="10px" color="green"></v-card>
                     </v-col>
                     <v-col cols="12" md="10">
                       <v-list two-line subheader class="ml-n8">
                  <v-list-item>
                    <v-list-item-content>
                       <v-list-item-subtitle>Blood</v-list-item-subtitle>
                      <v-list-item-title>A+</v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                </v-list>
                     </v-col>
                   </v-row>
                  </v-col>
                  <v-col cols="12" md="4">
                     <v-row>
                     <v-col cols="12" md="2">
                        <v-card height="50px" width="10px" color="red"></v-card>
                     </v-col>
                     <v-col cols="12" md="10">
                       <v-list two-line subheader class="ml-n8">
                  <v-list-item>
                    <v-list-item-content>
                       <v-list-item-subtitle>Height</v-list-item-subtitle>
                      <v-list-item-title>175 cm</v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                </v-list>
                     </v-col>
                   </v-row>
                  </v-col>
                  <v-col cols="12" md="4">
                    <v-row>
                     <v-col cols="12" md="2">
                        <v-card height="50px" width="10px" color="grey"></v-card>
                     </v-col>
                     <v-col cols="12" md="10">
                       <v-list two-line subheader class="ml-n8">
                  <v-list-item>
                    <v-list-item-content>
                       <v-list-item-subtitle>Weight</v-list-item-subtitle>
                      <v-list-item-title>64 kg</v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                </v-list>
                     </v-col>
                    </v-row>
                  </v-col>
                <v-col cols="12" sm="12">
                  <v-btn 
                      text
                      >November  
                    <v-icon right>   
                      mdi-chevron-down
                    </v-icon>
                  </v-btn>
                </v-col>
                <v-col cols="12" sm="12">
                    <v-list>
                <v-list-item >
                  <v-item-content>
                        <v-btn class="mr-1" outlined color="teal darken-1">MO</v-btn>
                  </v-item-content>
                   <v-item-content>
                        <v-btn class="mr-1" outlined color="teal darken-1">Tu</v-btn>
                  </v-item-content>
                   <v-item-content>
                        <v-btn class="mr-1" outlined color="teal darken-1">We</v-btn>
                  </v-item-content>
                   <v-item-content>
                        <v-btn  class="mr-1" color="teal darken-1" dark>Th</v-btn>
                  </v-item-content>
                  <v-item-content>
                        <v-btn  class="mr-1" outlined color="teal darken-1">Fr</v-btn>
                  </v-item-content>
                  <v-item-content>
                        <v-btn  class="mr-1" outlined color="teal darken-1">Sa</v-btn>
                  </v-item-content>
                  
                </v-list-item>
              </v-list>
                </v-col>
                <v-col cols="12" sm="12">
                    <v-card class="mx-12 rounded-tl-xl rounded-tr-xl rounded-bl-xl rounded-br-xl mt-n4 py-4" 
                    color="teal" dark flat>
                  <v-list-item three-line>
      <v-list-item-avatar
        tile
        size="30" 
      >
      <v-icon size="30">mdi-tooth</v-icon>
      </v-list-item-avatar>
      <v-list-item-content class="pa-2">
        <v-list-item-title class="headline mb-1">
          Dentist <br>
          <h6>8:00 - 9:30</h6> 
          <h6>Dr. Alex Brown(cab 39)</h6>
        </v-list-item-title>
      </v-list-item-content>
    </v-list-item>
  </v-card>
                </v-col>
                <v-col cols="12" sm="12">
                    <v-card class="mx-12 rounded-tl-xl rounded-tr-xl rounded-bl-xl rounded-br-xl mt-n4 py-4" 
                    color="teal lighten-5" flat>
                  <v-list-item three-line>
      <v-list-item-avatar tile size="30" >
              <v-icon size="30">fas fa-heartbeat</v-icon>
              </v-list-item-avatar>
              <v-list-item-content class="pa-2">
                <v-list-item-title class="headline mb-1">
                  Cardiologist <br>
                  <h6>9:45 - 11:50</h6> 
                  <h6>Dr. Elika Clark(cab 61)</h6>
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-card>
          
                </v-col>
                <v-col cols="12" sm="12">
                  <v-btn 
                      text
                      >Your Traitment  
                    <v-icon right>   
                      mdi-chevron-down
                    </v-icon>
                  </v-btn>
                </v-col>
                 <v-col cols="12" sm="12">
                    <v-card class="mx-12 rounded-tl-xl rounded-tr-xl rounded-bl-xl rounded-br-xl mt-n4 " 
                    color="teal lighten-5" flat>
                  <v-list-item three-line>
      <v-list-item-avatar tile size="30" >
              <v-icon size="30" color="teal">mdi-pill</v-icon>
              </v-list-item-avatar>
              <v-list-item-content class="pa-2">
                <v-list-item-title class="headline mb-1">
                  Gentle Iron <br>
                  <h6><span class="teal--text">2 capsules</span> with meals every day</h6> 
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-card>
          
                </v-col>
              </v-row>
          </v-container>
        </v-app>
      </v-flex>
    </v-layout>
  </v-app>
</template>
<script>
export default {
  data: () => ({
     width: 2,
      radius: 10,
      padding: 8,
      lineCap: 'round',
      value: [0, 2, 5, 9, 5, 10, 3, 5, 0, 0, 1, 8, 2, 9, 0],
      fill: false,
      type: 'trend',
      autoLineWidth: false,
  }),
  computed: {
    theme() {
      return this.$vuetify.theme.dark ? "dark" : "light";
    }
  },
  
};
</script>
<style scoped>

</style>
