<template>
  <v-app-bar flat app>
    <v-toolbar-title class="navTitle"
      ><span class="larger">B</span>LACK <span class="larger">H</span>ILLS
      <span class="larger">G</span>EAR</v-toolbar-title
    >

    <v-spacer></v-spacer>
    <v-toolbar-items>
      <v-btn text> Home </v-btn>
      <v-btn text> Store </v-btn>
      <v-btn text> About </v-btn>
      <v-btn text> Contact </v-btn>
    </v-toolbar-items>
  </v-app-bar>
</template>

<style scoped>
.navTitle {
  letter-spacing: 0.1em;
  font-weight: 600;
}
.larger {
  font-size: 130%;
}
</style>
