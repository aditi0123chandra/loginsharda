<template>
  <v-app class="light-blue darken-4">
    <v-content>
      <v-container class="fill-height" fluid>
        <v-row align="center" justify="center">
          <v-col cols="12" sm="8" md="8">
            <v-card class="elevation-12">
              <v-window v-model="step">
                <v-window-item :value="1">
                  <v-row>
                    <v-col cols="12" md="3" class="indigo darken-3"   align="center" justify="center">
                        <br>
                        <v-img src="../assets/book.png" class="indigo darken-3" height="150" width="150"></v-img>
                        <br>
                        <h2 class="white--text">LEARNSHALA</h2>
                    </v-col>
                    <v-col cols="12" md="8">
                      <v-card-text class="mt-12">
                        <h1 class="text-center display-2 indigo--text text--darken-3 font-weight-bold">Sharda Login</h1> <br>
                        <h4 class="text-center mlt-4 display-1 font-weight-bold">To access the facilities of Learnshala</h4>
                        <v-form>
                          <v-text-field
                          label="Email"
                          name="Email"
                          prepend-icon="email"
                          type="text"
                          color="indigo darken-3"
                          />
                          <v-text-field
                          id="password"
                          label="Password"
                          name="Password"
                          prepend-icon="lock"
                          type="password"
                          color="indigo darken-3"
                          />
                        </v-form>
                        <div class="text-center mt-3">
                          <v-btn rounded color="indigo darken-3" dark>LOG IN</v-btn>
                        </div>
                        <h3 class="text-center mt-3"><a href="about">Forgot Password?</a></h3>
                      </v-card-text>
                      
                    </v-col>
                    
                  </v-row>

                </v-window-item>
                <v-window-item :value="2">

                </v-window-item>
              </v-window>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    step: 1
  }),
  props: {
    source: String
  }
}
</script>