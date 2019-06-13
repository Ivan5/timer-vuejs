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
      <v-list>
        <v-list-tile
          v-for="(lap,index) in laps"
          :key="index"
        >Lap {{index + 1 }} : {{ lap.formattedTime }}</v-list-tile>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  props: ["laps"],
  data() {
    return {
      isDrawerOpen: false
    };
  }
};
</script>

<style>
</style>
