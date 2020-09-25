<template>
  <!-- App.vue -->

  <v-app>
    <v-navigation-drawer app v-if="drawer">
      <!-- -->
    </v-navigation-drawer>

    <v-app-bar app color="#970747" dark>
      <v-app-bar-nav-icon to="/"></v-app-bar-nav-icon>

      <v-toolbar-title>UNET WORLD</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-toolbar-items class="mr-n4">
        <v-btn to="/signup" text>Sign Up</v-btn>
        <v-btn to="/login" text>Log In</v-btn>
      </v-toolbar-items>
    </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>
      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <!-- If using vue-router -->
        <router-view />
      </v-container>
    </v-main>

    <v-footer app color="#970747" dark fixed>
      <v-spacer></v-spacer>
      <div>Unet World &copy; {{ new Date().getFullYear() }}</div>
      <v-spacer></v-spacer>
    </v-footer>
  </v-app>
</template>

<script>
//import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",

  components: {
    //HelloWorld,
  },

  data: () => ({
    drawer: false,
  }),
};
</script>
<style>
h1 {
  color: #970747;
}

p {
  color: #970747;
}
</style>
