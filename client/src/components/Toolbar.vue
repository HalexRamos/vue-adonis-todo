<template>
  <v-toolbar color="green" dark fixed>
    <v-toolbar-title class="mr-4">VUE TODO</v-toolbar-title>
    <v-toolbar-items>
      <v-btn flat>
        <v-icon class="mr-2">playlist_add_check</v-icon>
        Projects
      </v-btn>
    </v-toolbar-items>
    <v-spacer></v-spacer>
    <v-toolbar-items class="hidden-sm-and-down">
      <v-btn to="/register" flat>
        <v-icon class="mr-2">account_box</v-icon>
        Register
      </v-btn>
      <v-btn flat>
        <v-icon class="mr-2" to="/">fingerprint</v-icon>
        Login
      </v-btn>
      <v-btn flat>
        <v-icon class="mr-2">exit_to_app</v-icon>
        Logout
      </v-btn>
      <v-btn flat>
        <v-icon class="mr-2">ondemand_video</v-icon>
        How this is made
      </v-btn>
    </v-toolbar-items>
  </v-toolbar>
</template>

<script>
export default {};
</script>

<style>
</style>
