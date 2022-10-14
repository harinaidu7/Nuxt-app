<template>
    <div>
        <nav>
            <v-app dark>
                <v-app-bar app elivation="3" class="indigo lighten-1" >
                    <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
                    <v-toolbar-title><span class="text-upper">Task</span><v-icon>mdi-24px mdi-attachment</v-icon><span>Manager</span></v-toolbar-title>
                    <v-spacer></v-spacer>
                    <!-- <Nuxt-link  style="text-decoration: none; color: inherit;" to="/Login" > -->
                        <!-- <v-btn class="indigo lighten-3"><span>login</span><v-icon>mdi-login-variant</v-icon></v-btn> -->
                        <Signup/>
                    <!-- </Nuxt-link> -->
                </v-app-bar>
                <v-navigation-drawer app  v-model="drawer" class=" indigo lighten-1 pa-10">
                    <v-avatar size="100">
                        <img src="../assets/profile2.jpeg"/>
                    </v-avatar>  
                    <v-spacer></v-spacer>
                    <v-list>
                        <v-list-title>
                          
                            <v-list-tile-action>
                              <v-icon class="black--text">mdi-view-dashboard</v-icon>
                            </v-list-tile-action>
                            <v-list-title-content>
                              <v-list-title-title >Dashboard</v-list-title-title>
                            </v-list-title-content>
                            <v-spacer></v-spacer>

                            <v-list-tile-action>
                                <v-icon class="black--text">mdi-folder-account</v-icon>
                              </v-list-tile-action>
                              <v-list-title-content>
                                <v-list-title-title >My Project</v-list-title-title>
                              </v-list-title-content>
                              <v-spacer></v-spacer>

                              <v-list-tile-action>
                                <v-icon class="black--text">mdi-account</v-icon>
                              </v-list-tile-action>
                              <v-list-title-content>
                                <v-list-title-title >Team</v-list-title-title>
                              </v-list-title-content>
                              <v-spacer></v-spacer>
          
                          
                        </v-list-title>
                      </v-list>
                     
                        

                    
                    
                   
                    
                </v-navigation-drawer>

                
            </v-app>

        </nav>

    </div>
</template>

<script>
import Signup from './Signup.vue';
    export default {
    components: {  Signup },
    data(){
        return{
            drawer:false
        }
    },
    methods:{
        
    }
}
</script>

<style scoped>

</style>