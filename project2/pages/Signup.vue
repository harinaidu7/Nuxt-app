<template>
    <div>
        <!-- <p>Login!!!</p> -->
        <v-dialog max-width="600px" v-if="!login">
            <!-- login button -->
            <template  v-slot:activator="{ on, attrs }">
                <v-btn v-bind="attrs" v-on="on" flat slot="activator" class="indigo lighten-3" >Sign up<v-icon>mdi-account-plus</v-icon></v-btn>
            </template>
            <!-- login button end-->

            <v-card>
                <v-card-title>
                    <h2>Sign up to get started</h2>
                </v-card-title>
                <v-card-text>
                    <v-form calss="px-3" ref="form">
                        <v-text-field label="First name" prepend-icon="mdi-account" v-model="fname"></v-text-field>
                        <v-text-field label="Last Name" prepend-icon="mdi-account" v-model="lname"></v-text-field>
                        <v-text-field label="Phone No" prepend-icon="mdi-cellphone" v-model="phoneno"></v-text-field>
                        <v-text-field label="Email Id" prepend-icon="mdi-email" v-model="email"></v-text-field>
                        <v-text-field label="Password" prepend-icon="mdi-key-variant" v-model="password"></v-text-field>
                        <v-text-field label="Confirm Password" prepend-icon="mdi-key-variant" v-model="cpassword"></v-text-field>
                        <v-flex class="d-flex justify-center">
                            <v-btn class="indigo darken-1">Submit</v-btn>
                        </v-flex>
                        <v-flex class="d-flex justify-center">
                            <h4>Already a user ? please <span><v-btn  small class="ma-3 " outlined color="black" @click="login =!login">Login</v-btn></span></h4>
                        </v-flex>
                        


                    </v-form>
                </v-card-text>
            </v-card>
        </v-dialog>

        <v-dialog max-width="600px" v-if="login">
            <!-- login button -->
            <template  v-slot:activator="{ on, attrs }">
                <v-btn v-bind="attrs" v-on="on" flat slot="activator" class="indigo lighten-3" >Sign up<v-icon>mdi-account-plus</v-icon></v-btn>
            </template>
            <!-- login button end-->

            <v-card>
                <v-card-title>
                    <h2>Login</h2>
                </v-card-title>
                <v-card-text>
                    <v-form calss="px-3" ref="form">
                        <v-text-field label="Email Id" prepend-icon="mdi-email" v-model="email"></v-text-field>
                        <v-text-field label="Password" prepend-icon="mdi-key-variant" v-model="password"></v-text-field>
                        <v-flex class="d-flex justify-center">
                            <v-btn class="indigo darken-1">Submit</v-btn>
                        </v-flex>
                        <!-- <v-flex class="d-flex justify-center">
                            <h4>Already a user ? please <span><v-btn flat @click="login">Login</v-btn></span></h4>
                        </v-flex> -->
                        


                    </v-form>
                </v-card-text>
            </v-card>
        </v-dialog>
        
    </div>
</template>

<script>
    export default {
        name:'Login',
        dialog:false,
        data(){
            return{
                login:false
            }
        },
        
    
    }
</script>

<style scoped>

</style>