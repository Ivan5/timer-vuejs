<template>
  <nav>
    <v-toolbar app dark class="secondary">
      <v-toolbar-side-icon @click="isDrawerOpen = !isDrawerOpen"></v-toolbar-side-icon>
      <v-toolbar-title class="headline text-uppercase">
        <span class="font-weight-black primary--text">Ivan's</span>
        <span class="font-weight-light">Timer</span>
      </v-toolbar-title>
    </v-toolbar>

    <v-navigation-drawer dark app v-model="isDrawerOpen">
      <v-toolbar class="secondary">
        <v-toolbal-title class="title">Laps</v-toolbal-title>
      </v-toolbar>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      isDrawerOpen: false
    };
  }
};
</script>

<style>
</style>
