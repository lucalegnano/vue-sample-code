<template>
  <transition name="fade" mode="out-in">
    <v-container class="fill-height about">
      <div class="page">
        <v-row class="mx-2 my-4">
          <v-col cols="auto" class="display-2 pa-1">
              <span class="blue--text">M</span>
              <span class="font-weight-light">uhammad</span>
          </v-col>
          <v-col cols="auto" class="display-2 pa-1">
              <span class="blue--text">R</span>
              <span class="font-weight-light">ubaiyat</span>
          </v-col>
        </v-row>
        <v-row no-gutters class="mx-2 px-2 my-2">
          <v-col cols="auto">Mover of Bits</v-col>
          <v-col cols="auto" class="blue--text mx-3 font-weight-black">|</v-col>
          <v-col cols="auto">Arranger of Pixels</v-col>
        </v-row>
        <v-row no-gutters class="mx-2 px-2 my-2">
          <v-col cols="auto">Likes to work with cutting-edge technologies to solve interesting problems</v-col>
        </v-row>
        <v-row no-gutters class="mx-2 px-2 my-2">
          <v-col cols="auto">Based on Dhaka</v-col>
           <v-col cols="auto"  class="blue--text mx-2 font-weight-black">/</v-col> 
          <v-col>Bangladesh</v-col>
        </v-row>

        <v-row class="mx-1">
          <v-col cols="auto" class="mx-0 px-1 py-0">
              <v-hover v-slot:default="{ hover }">
                <v-btn 
                  text 
                  tile 
                  max-width="90" 
                  v-bind:class="hover ? 'blue--text' : 'white--text'"
                  v-on:click="openLinkedIn"
                >
                  LinkedIn
                </v-btn>
              </v-hover>
          </v-col>
          <v-col cols="auto" class="mx-0 pa-0">
              <v-hover v-slot:default="{ hover }">
                <v-btn 
                  text 
                  tile 
                  max-width="90" 
                  v-bind:class="hover ? 'blue--text' : 'white--text'"
                  v-on:click="openGithub"
                >
                  Github
                </v-btn>
              </v-hover>
          </v-col>
          <v-col cols="auto" class="mx-0 pa-0">
              <v-hover v-slot:default="{ hover }">
                <v-btn 
                  text 
                  tile 
                  max-width="90" 
                  v-bind:class="hover ? 'blue--text' : 'white--text'"
                  v-on:click="mailZyrif"
                >
                  Email
                </v-btn>
              </v-hover>
          </v-col>
        </v-row>
      </div>
    </v-container>
  </transition>
</template>

<script>
export default {
  methods: {
    openLinkedIn() {
      window.open("https://www.linkedin.com/in/clementi/", "_blank")
    },
    openGithub() {
      window.open("https://github.com/clementi", "_blank")
    },
    mailZyrif() {
      window.open("mailto:clementi@luca.net", "_blank")
    }
  }
};
</script>

<style>
.container.about {
  background-color: #222;
}
</style>