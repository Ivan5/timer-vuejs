<template>
  <v-app>
    <Navbar/>
    <v-content>Hello World</v-content>
  </v-app>
</template>

<script>
import Navbar from "./components/Navbar.vue";
export default {
  name: "App",
  components: {
    Navbar
  },
  data() {
    return {
      //
    };
  }
};
</script>
