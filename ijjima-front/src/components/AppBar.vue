<script setup>
import { ref } from 'vue'

const title = ref('The Funny Dudes')
</script>

<template>
  <v-app-bar app class="elevation-0 text-white" fixed color="transparent">
    <v-row>
      <v-col cols="4" align="center">
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
      </v-col>
      <v-col cols="4" align="center">
        <h1 flex centered class="title">{{ title }}</h1>
      </v-col>
      <v-col cols="4" align="center">
        <v-btn icon="mdi-spotify" href="https://open.spotify.com/playlist/0PWhB1LKuxePCF5F5p48yC" target="_blank"></v-btn>
        <v-btn icon="mdi-instagram" ></v-btn>
      </v-col>
    </v-row>
  </v-app-bar>
</template>
<style scoped>
.title {
  font-family: 'Sedgwick Ave Display', cursive;
  font-size: 30px;
}
</style>
