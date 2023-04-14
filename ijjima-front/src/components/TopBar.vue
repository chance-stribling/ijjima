<script>
export default {
  data() {
    return {
      title: 'G59'
    }
  }
}
</script>
<template>
  <v-app-bar app theme="dark" density="compact" hide-on-scroll>
    <v-app-bar-title>{{ title }}</v-app-bar-title>

    <template v-slot:append>
      <v-btn icon="mdi-dots-vertical"></v-btn>
    </template>
  </v-app-bar>
</template>
<style scoped></style>
