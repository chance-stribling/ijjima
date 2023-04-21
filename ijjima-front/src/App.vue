<script setup>
import { RouterView } from 'vue-router'
import AppBar from './components/AppBar.vue'
</script>

<template>
  <v-app>
    <AppBar />
    <v-main>
      <RouterView />
    </v-main>
  </v-app>
  <div class="circle"></div>
</template>

<style scoped></style>
