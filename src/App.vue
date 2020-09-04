<template>
  <v-app>
    <v-app-bar app color="info" dark>
      <v-toolbar-title>Vue with Vuetify</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn to="/home" text>Home</v-btn>
      <v-btn to="/"
      color="deep-purple accent-4"
      class="rounded-xl">Login</v-btn>
    </v-app-bar>

    <v-main>
      <router-view></router-view>
    </v-main>

    <v-footer
      class="font-weight-medium"
      color="light-blue darken-2"
    >
      <v-col
        class="text-center"
        cols="12"
      >
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </v-col>
    </v-footer>
  </v-app>
</template>

<script>


export default {
  name: 'App',

  components: {
    
  },

  data: () => ({
    
  }),
};
</script>
