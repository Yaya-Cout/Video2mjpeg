<template>
  <v-btn icon @click="theme.cycle()">
    <v-icon>mdi-theme-light-dark</v-icon>
    <v-tooltip
      activator="parent"
      location="start"
    >Change theme</v-tooltip>
  </v-btn>
</template>

<script setup lang="ts">
  import { useTheme } from 'vuetify'

  const theme = useTheme()
</script>

<style scoped>
</style>
