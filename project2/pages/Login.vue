<template>
    <div>
        <v-dialog max-width="600px">
            <!-- login button -->
            <template  v-slot:activator="{ on, attrs }">
            
                <!-- login button end-->
                
                <v-card slot="activator" v-bind="attrs"
                v-on="on">
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
                            
                        </v-form>
                    </v-card-text>
                </v-card>
            </template>
        </v-dialog>

    </div>
</template>

<script>
export default {
  name: "Login",
  dialog: false,
};
</script>

<style scoped>
</style>