<template>
  <v-app>
    <NavBar />
    <v-content class="black"><router-view></router-view></v-content>
  </v-app>
</template>

<script>
import NavBar from "./components/NavBar/NavBar";
export default {
  name: "App",

  components: { NavBar },

  data: () => ({
    //
  })
};
</script>
