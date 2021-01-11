<template>
  <v-app>
    <!-- tool bar -->
    <v-app-bar app color="green" dark>
      <!-- title -->
      <v-toolbar-title>GAS 家計簿</v-toolbar-title>
      <v-spacer></v-spacer>
      <!-- table icon button -->
      <v-btn icon to="/">
        <v-icon>mdi-file-table-outline</v-icon>
      </v-btn>
      <!-- gear icon button -->
      <v-btn icon to="/setting">
        <v-icon>mdi-cog</v-icon>
      </v-btn>
    </v-app-bar>
    <!-- main contents -->
    <v-main>
      <v-container fluid>
        <!-- router-view の中身がパスによって切り替わる -->
        <router-view></router-view>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'App'
}
</script>
